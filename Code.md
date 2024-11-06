``` Java
class Employee {
  private int employeeId;
  private String name;
  private String branch;
  private double rating;
  private boolean companyTransport;

  public Employee(int employeeId, String name, String branch, double rating, boolean companyTransport) {
    this.employeeId = employeeId;
    this.name = name;
    this.branch = branch;
    this.rating = rating;
    this.companyTransport = companyTransport;
  }

  public int getEmployeeId() { return employeeId; }
  public String getName() { return name; }
  public String getBranch() { return branch; }
  public double getRating() { return rating; }
  public boolean isCompanyTransport() { return companyTransport; }
}

class MyClass {
  public static int findCountOfEmployeesUsingCompTransport(Employee[] emps, String branch) {
    return (int)Arrays.stream(emps)
      .filter(e -> e.getBranch().equals(branch) && e.isCompanyTransport())
      .count();
  }

  public static Employee findEmployeeWithSecondHighestRating(Employee[] emps) {
    return Arrays.stream(emps)
      .filter(e -> !e.isCompanyTransport())
      .sorted((e1,e2) -> Double.compare(e2.getRating(), e1.getRating()))
      .skip(1)
      .findFirst()
      .orElse(null);
  }

  public static void main(String[] args) {
    Scanner sc = new Scanner(System.in);
    Employee[] emps = new Employee[4];

    for(int i=0; i<4; i++) {
      emps[i] = new Employee(
        sc.nextInt(),
        sc.next(),
        sc.next(),
        sc.nextDouble(),
        sc.nextBoolean()
      );
    }

    String branch = sc.next();

    int count = findCountOfEmployeesUsingCompTransport(emps, branch);
    System.out.println(count > 0 ? count : "No such Employees");

    Employee emp = findEmployeeWithSecondHighestRating(emps);
    if(emp != null) {
      System.out.println(emp.getEmployeeId());
      System.out.println(emp.getName());
    } else {
      System.out.println("All Employees using company transport");
    }
  }
}



-----



class AutonomousCar {
  private int carId;
  private String brand;
  private int noOfTestsConducted;
  private int noOfTestsPassed;
  private String environment;
  private String grade;

  public AutonomousCar(int carId, String brand, int noOfTestsConducted, int noOfTestsPassed, String environment) {
    this.carId = carId;
    this.brand = brand;
    this.noOfTestsConducted = noOfTestsConducted;
    this.noOfTestsPassed = noOfTestsPassed;
    this.environment = environment;
  }

  public int getCarId() { return carId; }
  public void setCarId(int carId) { this.carId = carId; }
  public String getBrand() { return brand; }
  public void setBrand(String brand) { this.brand = brand; }
  public int getNoOfTestsConducted() { return noOfTestsConducted; }
  public void setNoOfTestsConducted(int noOfTestsConducted) { this.noOfTestsConducted = noOfTestsConducted; }
  public int getNoOfTestsPassed() { return noOfTestsPassed; }
  public void setNoOfTestsPassed(int noOfTestsPassed) { this.noOfTestsPassed = noOfTestsPassed; }
  public String getEnvironment() { return environment; }
  public void setEnvironment(String environment) { this.environment = environment; }
  public String getGrade() { return grade; }
  public void setGrade(String grade) { this.grade = grade; }
}

class Solution {
  public static int findTestPassedByEnv(AutonomousCar[] cars, String env) {
    return Arrays.stream(cars)
      .filter(c -> c.getEnvironment().equals(env))
      .mapToInt(AutonomousCar::getNoOfTestsPassed)
      .sum();
  }

  public static AutonomousCar updateCarGrade(AutonomousCar[] cars, String brand) {
    return Arrays.stream(cars)
      .filter(c -> c.getBrand().equals(brand))
      .findFirst()
      .map(c -> {
        double rating = (c.getNoOfTestsPassed() * 100.0) / c.getNoOfTestsConducted();
        c.setGrade(rating >= 80 ? "A1" : "B2");
        return c;
      })
      .orElse(null);
  }

  public static void main(String[] args) {
    Scanner sc = new Scanner(System.in);
    AutonomousCar[] cars = new AutonomousCar[4];

    for(int i=0; i<4; i++) {
      cars[i] = new AutonomousCar(
        sc.nextInt(),
        sc.next(),
        sc.nextInt(),
        sc.nextInt(),
        sc.next()
      );
    }

    String env = sc.next();
    String brand = sc.next();

    int totalPassed = findTestPassedByEnv(cars, env);
    System.out.println(totalPassed > 0 ? totalPassed : "There are no tests passed in this particular environment");

    AutonomousCar car = updateCarGrade(cars, brand);
    System.out.println(car != null ? car.getBrand() + "::" + car.getGrade() : "No Car is available with the specified brand");
  }
}



-------------------------



class Course {
  private int courseId;
  private String courseName;
  private String courseAdmin;
  private int quiz;
  private int handson;

  public Course(int courseId, String courseName, String courseAdmin, int quiz, int handson) {
    this.courseId = courseId;
    this.courseName = courseName;
    this.courseAdmin = courseAdmin;
    this.quiz = quiz;
    this.handson = handson;
  }

  public int getCourseId() { return courseId; }
  public void setCourseId(int courseId) { this.courseId = courseId; }
  public String getCourseName() { return courseName; }
  public void setCourseName(String courseName) { this.courseName = courseName; }
  public String getCourseAdmin() { return courseAdmin; }
  public void setCourseAdmin(String courseAdmin) { this.courseAdmin = courseAdmin; }
  public int getQuiz() { return quiz; }
  public void setQuiz(int quiz) { this.quiz = quiz; }
  public int getHandson() { return handson; }
  public void setHandson(int handson) { this.handson = handson; }
}

class CourseProgram {
  public static int findAvgOfQuizByAdmin(Course[] courses, String admin) {
    return (int)Arrays.stream(courses)
      .filter(c -> c.getCourseAdmin().equals(admin))
      .mapToInt(Course::getQuiz)
      .average()
      .orElse(0);
  }

  public static Course[] sortCourseByHandsOn(Course[] courses, int handson) {
    Course[] filtered = Arrays.stream(courses)
      .filter(c -> c.getHandson() < handson)
      .sorted((c1, c2) -> Integer.compare(c1.getHandson(), c2.getHandson()))
      .toArray(Course[]::new);
    return filtered.length > 0 ? filtered : null;
  }

  public static void main(String[] args) {
    Scanner sc = new Scanner(System.in);
    Course[] courses = new Course[4];

    for(int i=0; i<4; i++) {
      courses[i] = new Course(
        sc.nextInt(),
        sc.next(),
        sc.next(),
        sc.nextInt(),
        sc.nextInt()
      );
    }

    String admin = sc.next();
    int handson = sc.nextInt();

    int avg = findAvgOfQuizByAdmin(courses, admin);
    System.out.println(avg > 0 ? avg : "No Course found");

    Course[] sorted = sortCourseByHandsOn(courses, handson);
    if(sorted != null) {
      for(Course c : sorted) {
        System.out.println(c.getCourseName());
      }
    } else {
      System.out.println("No Course found with mentioned attribute");
    }
  }
}


----


class Movie {
  private String movieName;
  private String company;
  private String genre;
  private int budget;

  public Movie(String movieName, String company, String genre, int budget) {
    this.movieName = movieName;
    this.company = company;
    this.genre = genre;
    this.budget = budget;
  }

  public String getMovieName() { return movieName; }
  public void setMovieName(String movieName) { this.movieName = movieName; }
  public String getCompany() { return company; }
  public void setCompany(String company) { this.company = company; }
  public String getGenre() { return genre; }
  public void setGenre(String genre) { this.genre = genre; }
  public int getBudget() { return budget; }
  public void setBudget(int budget) { this.budget = budget; }
}

class MovieSolution {
  public static Movie[] getMovieByGenre(Movie[] movies, String searchGenre) {
    return Arrays.stream(movies)
      .filter(m -> m.getGenre().equalsIgnoreCase(searchGenre))
      .toArray(Movie[]::new);
  }

  public static void main(String[] args) {
    Scanner sc = new Scanner(System.in);
    Movie[] movies = new Movie[4];

    for(int i=0; i<4; i++) {
      movies[i] = new Movie(
        sc.next(),
        sc.next(),
        sc.next(),
        sc.nextInt()
      );
    }

    String searchGenre = sc.next();

    Arrays.stream(getMovieByGenre(movies, searchGenre))
      .forEach(m -> System.out.println(m.getBudget() > 80000000 ?
        "High Budget Movie" : "Low Budget Movie"));
  }
}


------


class Student {
  private int id;
  private String name;
  private int totalMarksObt;

  public Student(int id, String name, int totalMarksObt) {
    this.id = id;
    this.name = name;
    this.totalMarksObt = totalMarksObt;
  }

  public int getId() { return id; }
  public String getName() { return name; }
  public int getTotalMarksObt() { return totalMarksObt; }
}

class Solution {
  public static void findStudentWithHighestTotal(Student[] students) {
    System.out.println(Arrays.stream(students)
      .max((s1, s2) -> Integer.compare(s1.getTotalMarksObt(), s2.getTotalMarksObt()))
      .map(s -> s.getName().toUpperCase())
      .orElse(""));
  }

  public static List<Integer> searchStudentByPercentage(Student[] students) {
    List<Integer> result = Arrays.stream(students)
      .filter(s -> s.getTotalMarksObt() / 4 >= 70)
      .map(Student::getId)
      .sorted()
      .collect(Collectors.toList());

    return result.isEmpty() ? null : result;
  }

  public static void main(String[] args) {
    Scanner sc = new Scanner(System.in);
    int n = sc.nextInt();
    Student[] students = new Student[n];

    for(int i=0; i<n; i++) {
      students[i] = new Student(
        sc.nextInt(),
        sc.nextLine().trim(),
        sc.nextInt()
      );
    }

    System.out.println();

    findStudentWithHighestTotal(students);

    List<Integer> result = searchStudentByPercentage(students);
    if(result != null) {
      result.forEach(System.out::println);
    } else {
      System.out.println("No Student found with mentioned attribute.");
    }
  }
}
```
