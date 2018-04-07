# Project 7 - WordPress Pentesting

Time spent: 4 hours spent in total

> Objective: Find, analyze, recreate, and document three vulnerabilities affecting an old version of WordPress

## Pentesting Report

1.  WordPress <= 4.2.2 - Authenticated Stored Cross-Site Scripting (XSS)
		ID:CVE-2015-5622 
  - [ ] Summary: 
    - Vulnerability types: XSS
    - Tested in version: 4.2
    - Fixed in version: 4.2.3 
  - [ ] GIF Walkthrough: <img src="https://github.com/CTUDEV/Web-Security-Week-7-Project-WordPress-vs.-Kali/blob/master/EXP1.%20XSS.gif" width="800">
  - [ ] Steps to recreate: Create a new post and insert the code from the link as the body of the post. Publish the post.
  - [Link 1](https://klikki.fi/adv/wordpress3.html)

1. WordPress 3.6.0-4.7.2 - Authenticated Cross-Site Scripting (XSS) via Media File Metadata
              ID:CVE-2017-6814

  - [ ] Summary: 
    - Vulnerability types: XSS
    - Tested in version: 4.2
    - Fixed in version: 4.2.13 
  - [ ] GIF Walkthrough:<img src="https://github.com/CTUDEV/Web-Security-Week-7-Project-WordPress-vs.-Kali/blob/master/EXP2.%20XSS.%20Audio%20FIle.gif" width="800">
  - [ ] Steps to recreate: Upload an mp3 audio file. Create an audio playlist with the uploaded file. Add the playlist to a post. Publish the post.    
  - [Link 1](http://seclists.org/oss-sec/2017/q1/563)
1. WordPress  4.0-4.7.2 - Authenticated Stored Cross-Site Scriptin   (XSS) in YouTube URL Embeds
	 ID:CVE-2017-6817
- [ ] Summary: 
    - Vulnerability types:XSS
    - Tested in version:4.2
    - Fixed in version:4.2.13 
  - [ ] GIF Walkthrough:<img src="https://github.com/CTUDEV/Web-Security-Week-7-Project-WordPress-vs.-Kali/blob/master/EXP3.%20XSS.%20YouTube.gif" width="800">
  - [ ] Steps to recreate:
	Create a new post where we insert the following:[embed src='https://youtube.com/embed/12345\x3csvg onload=alert(1)\x3e'][/embed] as the body of the post. Publish the post. 
  - [Link 1](https://blog.sucuri.net/2017/03/stored-xss-in-wordpress-core.html)


## Assets

No additional assets.

## Resources

- [WordPress Source Browser](https://core.trac.wordpress.org/browser/)
- [WordPress Developer Reference](https://developer.wordpress.org/reference/)

GIFs created with [LiceCap](http://www.cockos.com/licecap/).

## Notes

No challenges were encountered while doing the work.


## License

    Copyright 2018 Oleksandr Kozlenko

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
