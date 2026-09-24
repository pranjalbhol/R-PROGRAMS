1. year <- as.integer(readline(prompt = "Enter a year: "))

if ((year %% 4 == 0 && year %% 100 != 0) || (year %% 400 == 0)) {
  cat(year, "is a leap year.\n")
} else {
  cat(year, "is not a leap year.\n")
}


2. n <- as.integer(readline("Enter n: "))

if (n < 1) {
  print("Invalid")
} else {
  s <- 0
  while (n > 0) { s <- s + n; n <- n - 1 }
  cat("Sum:", s, "\n")
}


3. m <- as.numeric(readline(prompt = "Marks: "))

grade <- if (m >= 800) "A+" else if (m >= 700) "A" else if (m >= 500) "B+" else if (m >= 400) "B" else if (m >= 150) "C" else "D"

cat("Grade:", grade, "\n")


4. add <- function(a, b) a + b
sub <- function(a, b) a - b
mul <- function(a, b) a * b
div <- function(a, b) a / b

a <- as.numeric(readline("Enter num1: "))
b <- as.numeric(readline("Enter num2: "))
ch <- as.integer(readline("Choice (1-Add, 2-Sub, 3-Mul, 4-Div): "))

res <- switch(ch, add(a, b), sub(a, b), mul(a, b), div(a, b))
cat("Result:", res, "\n")



5. # Create matrix using rbind() and rename rows
MatrixOfTechnology <- rbind(
  Lang1 = c("C#", "Java", "Cobol", ".Net"),
  Lang2 = c("JavaScript", "NodeJs", "R", "Azure"),
  Lang3 = c("Power BI", "ASP.Net", "Unity", "Block Chain")
)

print(MatrixOfTechnology)

# Access element using row name
cat("Element:", MatrixOfTechnology["Lang2", 3], "\n")
