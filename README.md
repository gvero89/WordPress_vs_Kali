# WordPress_vs_Kali
# Project 7 - WordPress Pentesting
Time spent: **4** hours spent in total

> Objective: Find, analyze, recreate, and document **three vulnerabilities** affecting an old version of WordPress

## Pentesting Report
1. (Required) XSS in URL Embeds
  - [ ] Summary: 
    - Vulnerability types: Stored XSS in WP Core
    - Tested in version: 4.2
    - Fixed in version: 4.2.13
  - [ ] GIF Walkthrough:
  - [ ] Steps to recreate: Open up a new post and add an embedded YouTube video URL. In the URL, add an XSS at the end. For this example, "svg onload=alert(1)" was used to show a pop-up alert everytime the video would load. 
  
  - [ ] Affected source code:
    - [Link 1](https://github.com/WordPress/WordPress/commit/419c8d97ce8df7d5004ee0b566bc5e095f0a6ca8)
    
2. (Required) XSS in Embed YouTube URLs
  - [ ] Summary: 
    - Vulnerability types: XSS
    - Tested in version: 4.2
    - Fixed in version: 4.2.13
  - [ ] GIF Walkthrough: 
  - [ ] Steps to recreate: Open up a new post, and insert the embedded link for a YouTube video. At the end of the main embedded video statement, add an alert whenever the video loads. In this case, "onload=alert(123456789)" was the alert used. 
  - [ ] Affected source code:
    - [Link 2](https://github.com/WordPress/WordPress/commit/419c8d97ce8df7d5004ee0b566bc5e095f0a6ca8)

3. (Required) Stored XSS
  - [ ] Summary: 
    - Vulnerability types: XSS
    - Tested in version: 4.2 
    - Fixed in version: 4.2.3
  - [ ] GIF Walkthrough: 
  - [ ] Steps to recreate: Create a new post, and insert "a href="[caption code=">]</a><a title=" onmouseover=alert('test') ">link</a" in the body
  - [ ] Affected source code:
    - [Link 3](https://klikki.fi/adv/wordpress3.html)

## Assets

List any additional assets, such as scripts or files

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
