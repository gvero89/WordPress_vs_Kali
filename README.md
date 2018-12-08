# WordPress_vs_Kali
# Project 7 - WordPress Pentesting
Time spent: 25 hours spent in total

> Objective: Find, analyze, recreate, and document **three vulnerabilities** affecting an old version of WordPress

## Pentesting Report
1. Vulnerability: Stored XSS in WP
    In a Post XSS <script>alert(document.cookie);</script> in the comments section:
    
  - [ ] GIF Walkthrough: 
 
2. Vulnerability: Authenticated Stored Cross-Site Scripting
    Steps: Select Post -> Add new post -> <a onmouseover="alert('I got you!')">click here</a> -> click preview
    
  - [ ] GIF Walkthrough: 

3. Vulnerability: User Enumeration
    Steps: WordPress login page -> In admin write: username and password field will stay empty. 
           An Error will show: password field is empty.
           In admin write: username and in password: input any password.
           An Error will show: password you entered for the username admin is incorrect. 
           When a randomly username and password is added, shows the error which is invalid username.
           
  - [ ] GIF Walkthrough: 

## Resources

- [WordPress Source Browser](https://core.trac.wordpress.org/browser/)
- [WordPress Developer Reference](https://developer.wordpress.org/reference/)

## License

    Copyright [2018] [G. Veronica Juca]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
