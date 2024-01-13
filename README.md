#include <stdio.h>
#include <stdlib.h>
#include <math.h>

// Basic Operations
double add(double a, double b) { return a + b; }
double subtract(double a, double b) { return a - b; }
double multiply(double a, double b) { return a * b; }
double divide(double a, double b) { return a / b; }

// Trigonometric Operations
double sine(double angle) { return sin(angle); }
double cosine(double angle) { return cos(angle); }
double tangent(double angle) { return tan(angle); }
double arcsine(double value) { return asin(value); }
double arccosine(double value) { return acos(value); }
double arctangent(double value) { return atan(value); }

// Algebraic Operations
double exponentiation(double base, double exponent) { return pow(base, exponent); }
double squareRoot(double value) { return sqrt(value); }
double cubeRoot(double value) { return cbrt(value); }
double nthRoot(double value, double n) { return pow(value, 1.0 / n); }
double factorial(double n) { return (n == 0 || n == 1) ? 1 : n * factorial(n - 1); }
double absoluteValue(double value) { return fabs(value); }

// Logarithmic Operations
double logarithm(double value) { return log10(value); }
double naturalLogarithm(double value) { return log(value); }
double customBaseLogarithm(double value, double base) { return log(value) / log(base); }

// Statistical Operations
double mean(double data[], int n);
double median(double data[], int n);
int mode(int data[], int n);
double standardDeviation(double data[], int n);
double variance(double data[], int n);

// Additional Operations
int modulus(int a, int b);
double percentage(double value, double total);
int gcd(int a, int b);
int lcm(int a, int b);
double floorValue(double value);
double ceilValue(double value);

// Complex Number Operations
typedef struct {
    double real;
    double imag;
} Complex;

Complex addComplex(Complex a, Complex b);
Complex subtractComplex(Complex a, Complex b);
Complex multiplyComplex(Complex a, Complex b);
Complex divideComplex(Complex a, Complex b);
Complex conjugateComplex(Complex num);

// Matrix Operations
typedef struct {
    int rows;
    int cols;
    double **data;
} Matrix;

Matrix addMatrix(Matrix mat1, Matrix mat2);
Matrix subtractMatrix(Matrix mat1, Matrix mat2);

// Binary Operations
long long binaryAddition(long long binaryNum1, long long binaryNum2);
long long binarySubtraction(long long binaryNum1, long long binaryNum2);
long long binaryMultiplication(long long binaryNum1, long long binaryNum2);
long long binaryDivision(long long binaryNum1, long long binaryNum2);
long long binaryAND(long long binaryNum1, long long binaryNum2);
long long binaryOR(long long binaryNum1, long long binaryNum2);
long long binaryXOR(long long binaryNum1, long long binaryNum2);

// Engineering Operations
double lengthConversion(double value, char fromUnit, char toUnit);
double massConversion(double value, char fromUnit, char toUnit);
double temperatureConversion(double value, char fromUnit, char toUnit);
Complex polarToRectangular(double magnitude, double angle);
Complex rectangularToPolar(Complex num);

// Calculus Operations
double derivative(double (*func)(double), double x, double h);
double indefiniteIntegral(double (*func)(double), double a, double b, double dx);
double definiteIntegral(double (*func)(double), double a, double b, int numSegments);

int main() {
    // Example usage
    double a = 10.0, b = 5.0;
    printf("Addition: %.2f\n", add(a, b));
    printf("Subtraction: %.2f\n", subtract(a, b));
    printf("Multiplication: %.2f\n", multiply(a, b));
    printf("Division: %.2f\n", divide(a, b));

    double angle = 45.0;
    printf("Sine: %.2f\n", sine(angle));
    printf("Cosine: %.2f\n", cosine(angle));
    printf("Tangent: %.2f\n", tangent(angle));
    printf("Arcsine: %.2f\n", arcsine(0.5));
    printf("Arccosine: %.2f\n", arccosine(0.5));
    printf("Arctangent: %.2f\n", arctangent(1.0));

    // Continue adding other operations as needed

    return 0;
}
