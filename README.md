# Flowable Loan App – Setup Instructions

##Download
	# https://github.com/flowable/flowable-engine/releases
	Download the zip version of flowable you wish for the bar file is advised 6.8.1 Flowable
	
	#You could download other version however 6.8.1 works perfectly
	#other version might work but this ones work 100%
	Download - apache-maven-3.6.3-bin
			 - tomcat-9.0.41
			 - jdk-24_windows-x64_bin
	
## Installation Folders
- Install Java JDK 24 for Windows
- Install Apache Maven 9.0.41
- Unzip flowable.zip file downloaded

## Installation

1. **Install JDK and Maven**
   - Ensure `java -version` and `mvn -version` work in your terminal.

2. Copy the files from inside flowable-6.8.1\wars
   to tomcat-9.0.41\apache-tomcat-9.0.41\webapps

2. **Start Flowable UI**
   - Navigate to:
     ```
     Flowable/Installations/tomcat-9.0.41/apache-tomcat-9.0.41/bin
     ```
   - Run:
     - `startup.bat` (Windows)
     - `./startup.sh` (macOS/Linux)

3. **Access Applications**
   - URL: `http://localhost:8080/flowable-ui/`
   - Login: `admin`
   - Password: `test`

4. **Configure Maven (if needed)**
   - Add the `bin` directory of Maven to your system’s PATH.

5. **Import the BAR file**
   - In your browser, go to `http://localhost:8080/flowable-ui/`
   - Click the **App** tab in the top menu
   - Select **Import App**
   - Upload the `.bar` file located in:
     ```
     Flowable/Imports/
     ```

---

## Notes
- This project was built using Flowable 6.8.1 UI Modeler.
- Includes example BPMN workflows, DMN decision tables, Groovy script tasks, form definitions, and REST integration using custom Mocky endpoints.
- Users must create their own Mocky APIs. Example payloads are embedded in the script tasks for reference.

---

For any issues or questions, feel free to open an issue in the repository. Happy modeling!