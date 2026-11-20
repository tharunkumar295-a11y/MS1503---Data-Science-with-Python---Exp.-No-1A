# Experiment 1.A  Employee Data Display Using Python

## Aim

To collect employee details, validate inputs, and calculate gross and net salary using Python.

## Algorithm

1. **Start** the program.
2. **Read Employee Details** from the user:
   * Input `name` (String) for the employee's full name.
   * Input `emp_id` (String) for the employee's identification number.
   * Input `basic` (Float) for the employee's basic salary.
3. **Validate Input**:
   * Ensure `basic` is a valid numeric value and check if `basic < 0`. If invalid or negative, display an appropriate error message and terminate the program.
4. **Compute Allowances**:
   * Calculate House Rent Allowance: $\text{HRA} = 0.15 \times \text{basic}$.
   * Calculate Dearness Allowance: $\text{DA} = 0.10 \times \text{basic}$.
5. **Compute Gross Salary**:
   * Calculate total earnings before deductions: $\text{Gross Salary} = \text{basic} + \text{HRA} + \text{DA}$.
6. **Compute Tax Deduction**:
   * Calculate income tax at $8\%$ of gross pay: $\text{Tax} = 0.08 \times \text{Gross Salary}$.
7. **Compute Net Salary**:
   * Calculate take-home pay: $\text{Net Salary} = \text{Gross Salary} - \text{Tax}$.
8. **Display Formatted Payroll Report**:
   * Print a structured summary displaying `name`, `emp_id`, `basic`, `HRA`, `DA`, `Gross Salary`, `Tax`, and `Net Salary` formatted to two decimal places.
9. **Stop** the program.

## Program
# Define sample employee details
name = "John Doe"
emp_id = "EMP101"
basic = 50000.00

# Validate basic salary
if basic < 0:
    print("Error: Basic salary cannot be negative.")
else:
    # Calculate allowances
    hra = 0.15 * basic
    da = 0.10 * basic

    # Calculate gross salary
    gross_salary = basic + hra + da

    # Calculate tax deduction
    tax = 0.08 * gross_salary

    # Calculate net salary
    net_salary = gross_salary - tax

    # Display payroll report
    print("\n========== PAYROLL REPORT ==========")
    print(f"Employee Name : {name}")
    print(f"Employee ID   : {emp_id}")
    print(f"Basic Salary  : ₹{basic:.2f}")
    print(f"HRA (15%)     : ₹{hra:.2f}")
    print(f"DA (10%)      : ₹{da:.2f}")
    print(f"Gross Salary  : ₹{gross_salary:.2f}")
    print(f"Tax (8%)      : ₹{tax:.2f}")
    print(f"Net Salary    : ₹{net_salary:.2f}")
    print("====================================
except ValueError:
    print("Error: Please enter a valid numeric value for salary.")
## Output
<img width="462" height="198" alt="image" src="https://github.com/user-attachments/assets/054c2dac-15fa-48ac-a14e-c128a7c06600" />
## ✅ Result

The program successfully accepts and validates employee details, calculates allowances and deductions, and displays a well-formatted salary report.
