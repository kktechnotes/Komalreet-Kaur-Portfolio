---
nav_exclude: true
---

# Things to Improve in official Docker Docs
This topic lists the improvements that should be made in the official Docker documentation for better readability and understanding.
> **Note**: The list contains only a few of the gaps. After detailed analysis and content restructuring, an exhaustive list can be prepared.


1. Content Outline is neither user friendly nor readable. Please refer [Content Outline](./Content_Outline.md) topic for Installation to see an improved version.
2. The document is not divided based on perspective or Role-based. From basic to advance, every little detail is provided in one web file. <br/>
**Example**: 
	The roles can be Developers, Integration Engineers, Student, DevOps Engineer
4. The semantics of dividing a topic into Concept, Task and Reference information is not followed.
5. Information Flow in the TOC is incorrect <br/>
**Example**: 
	- System Requirements should be explained before Installation Steps
	- Prerequisites to run the Docker Desktop are missing. For example, WSL2 is mandatory but it is mentioned in another topic. The Virtualization concept is also explained in another topic. 
5. The Headings are ambiguous and not meaningful.<br/>
**Example**: 
    - In TOC, the headings are "Mac", "Windows" and "Linux." It should have been *Installing Docker on Windows*, *Installing Docker on Linux*, *Installing Docker on Mac*
    - In the *Install Docker Desktop on Windows* topic, the heading "Install interactively" is meaningless. It should have been *Install Docker through GUI*
 5. Technical Writing Standards are not followed while writing the content. <br/>
 **Example**: 
	-	In *Install Docker Desktop on Windows* procedure, the following things are not as per [MSTP](https://docs.microsoft.com/en-us/style-guide/welcome/) writing style:
		-	The file name is mentioned without a link. For example, Docker Desktop Installer.exe
		-	Important Tips or Notes are part of the step itself. This impacts readability and the procedure no longer remains action-oriented
		-	The procedure does not contain Step Result, Final Result, Prerequisites, Context information or Lead sentence 
		-	In the *Install from the command line* procedure, the flag options are explained within the procedure. Explaining through choice table would have increased the readability.
	- Lack of parallelism in the content and TOC structure. 
6. Use of Incorrect English and Grammar throughout the content
**Example**:
	- Incorrect preposition used, than v/s to. The content contains, "If your admin account is different to your user account"
	- After explicitly mentioning the topic **About Windows containers**, the lead line contains interrogative statement "Looking for information on using Windows containers?"
