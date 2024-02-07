<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Student Grade Lookup</title>
    <script>
        function getStudentInfo() {
            var studentId = document.getElementById("studentId").value;
            google.script.run.withSuccessHandler(updateStudentInfo).getStudentInfo(https://script.google.com/macros/s/AKfycbx9rh8AGF1EKBqLMFn-ex9sG6XzM3JTWGUBVTzN9suUQW95UXQr9BgMJ7Lqf4eaTj4aYQ/exec);
        }

        function updateStudentInfo(studentInfo) {
            document.getElementById("name").innerText = studentInfo.name;
            document.getElementById("grade").innerText = studentInfo.grade;
        }
    </script>
</head>
<body>
    <h1>Student Grade Lookup</h1>
    <label for="studentId">Enter your ID number:</label>
    <input type="text" id="studentId">
    <button onclick="getStudentInfo()">Submit</button>
    <p>Your name: <span id="name"></span></p>
    <p>Your grade: <span id="grade"></span></p>
</body>
</html>
