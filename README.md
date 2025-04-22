# MPIN_strength_check
This project offers a comprehensive analysis of the strength of 4-digit and 6-digit MPINs used to access mobile banking apps, taking into account both commonly used MPINs and demographic trends based on their personal data such as their DOB,Wedding Anniversary or Spouse birthday.
🔍 Code Functionality and Algorithm Description
✅ Main Function:
commonly_used_mpin(mpin)
This function evaluates whether an MPIN is considered common or weak based on several pattern checks. It is useful in contexts where you want to enhance security validation for user-selected PINs.
📌 Checks Performed:
1.Pattern-Based Analysis:
   Detects weak or predictable patterns:
       - Repeating digits (e.g., 1111, 000000)
       - Ascending/descending sequences (e.g., 1234, 987654)
       - Palindromes (e.g., 1221, 4554)
       - Repeated blocks (e.g., 1212, 343434)
2.Demographic-Based Analysis:
   - Analyzes MPIN usage patterns abased on their personal data such as their DOB,Wedding Anniversary or Spouse birthday .
3.Date Format Handling (New Feature):
    -The program now handles multiple date formats (e.g., dd-mm-yyyy, yyyy-mm-dd, mm/dd/yyyy etc.). The program automatically identifies and processes the date format, ensuring it correctly      interprets the input. However there are some limitations as no third party libraries are used:
    - It assumes the most common format used in India which is dd/mm/yyyy.
    - It tries to detect which part corresponds to day, month and year and based on location it assumes a particular date format.

⚙️ Setup
1.Clone this repository:
  git clone https://github.com/your-username/mpin-pattern-analyzer.git
2.Open the notebook:
  Using Jupyter Notebook or any IDE that supports .ipynb files.

🛡️ Use Case
>>Mobile Banking & FinTech Apps: Validate user-selected MPINs before accepting them.
>>Authentication Systems: Reduce the risk of brute force attacks by preventing weak PINs.

