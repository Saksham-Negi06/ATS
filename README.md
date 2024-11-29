##Resume Validator

This script performs basic validation checks on a resume file to ensure that it includes essential sections and details such as name, email, phone number, education, project details, work experience, and skills.

Features

The script:
	1.	Extracts text from resumes in PDF or DOCX format.
	2.	Validates the presence of key sections and details:
	•	Name
	•	Email
	•	Phone number
	•	Education details
	•	Project details
	•	Work experience
	•	Skills
	3.	Displays the validation results in a tabular format using the tabulate library.

Requirements

	•	Python 3.6 or above
	•	Libraries:
	•	re
	•	docx2txt
	•	pdfplumber
	•	tabulate

You can install the required libraries using pip:

pip install docx2txt pdfplumber tabulate

Usage

	1.	Clone or download this repository.
	2.	Run the script:

python resume_validator.py


	3.	Provide the path to the resume file when prompted. Supported formats are .pdf and .docx.

Output

The script outputs a table indicating whether each key section or detail is present in the resume:

+------+-------------------+---------+
| S.No | Resume Details    | Yes/No  |
+------+-------------------+---------+
| 1    | Name              | Yes     |
| 2    | E-mail            | No      |
| 3    | Phone Number      | Yes     |
| 4    | Educational Check | Yes     |
| 5    | Project Details   | No      |
| 6    | Work Experience   | Yes     |
| 7    | Skills            | Yes     |
+------+-------------------+---------+

Functionality

Validation Checks

	•	Name Check: Verifies if the name follows the format of a proper noun (e.g., “John Doe”).
	•	Email Check: Validates email format.
	•	Phone Number Check: Ensures the presence of a country code and a 10-digit number.
	•	Education Check: Checks for year, institution/university name, and percentage/grade.
	•	Project Check: Ensures the presence of a section mentioning projects.
	•	Experience Check: Verifies work experience details.
	•	Skill Check: Confirms if a skills section exists.

File Handling

	•	Extracts text from .pdf files using pdfplumber.
	•	Extracts text from .docx files using docx2txt.

Limitations

	•	The script uses regular expressions for validation, which might not account for all edge cases.
	•	It does not support file formats other than .pdf and .docx.

License

This project is licensed under the MIT License. See the LICENSE file for details.

Feel free to contribute by submitting issues or pull requests!
