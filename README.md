# DSC180A-Quarter1-Integration

## Instructions for accessing AWS on a local machine.

1. Open terminal and clone this repo <br>
2. Navigate to the repository directory: <br>
```cd DSC180A-Quarter1-Integration```<br>

3. Use the following commands to gain access to the AWS server:<br>
``` chmod 0400 med1.pem ``` <br>
``` ssh -i med1.pem ubuntu@54.186.34.136 ``` <br>
(Make sure the file name is **"med1.pem"** with **"pem"** extension instead of other file extension)<br>

4. Follow these commands to connect to the Jupyter notebook:<br>
``` sudo snap install jupyter ``` <br>
``` jupyter notebook --port=<4-digit-number> ```<br>
For **<4-digit-number>**,avoid using 8888 and try using other ports.<br>
After executing these commands, you will see the following response:<br>
<img width="569" alt="image" src="https://github.com/PatrickTangwen/DSC180A-Quarter1-Integration/assets/102566928/8db3a9a6-40c0-4891-abe2-2139c7da5b14"> <br>

5. Copy the URL displayed at the bottom:<br>
For example, the URL displayed at the bootom of the screenshot is:<br>
```http://localhost:8886/?token=5d4bea140a359144f1fbe969e9251c8bc5d546329c7b46f4```
(You should have a different URL)

6. Open a new browser tab and paste the  URL into the address bar.<br>

7. Open a new terminal and navigate to the same repository directory:
   ```cd DSC180A-Quarter1-Integration```<br>
   Then, in the terminal, type the following command:
   ``` ssh -i med1.pem ubuntu@54.186.34.136 -L <4-digit-number>:localhost:<4-digit-number> ```<br>
   For **<4-digit-number>**, avoid using 8888 and try using other ports. Use the same port number as in the **step4**
   
8. Refresh the page from **step 5**, and you should now be able to access the Jupyter notebook.
