# DSC180A-Quarter1-Integration

## Instructions for accessing AWS on a local machine.

1. Open terminal and clone this repository using the following command: <br>
```git clone https://github.com/PatrickTangwen/DSC180A-Quarter1-Integration.git```

3. Navigate to the repository directory: <br>
```cd DSC180A-Quarter1-Integration```<br>

4. Use the following commands to gain access to the AWS server:<br>
``` chmod 0400 med1.pem ``` <br>
``` ssh -i med1.pem ubuntu@54.186.34.136 ``` <br>
(Make sure the file name is **"med1.pem"** with **"pem"** extension instead of other file extension)<br>

5. Follow these commands to connect to the Jupyter notebook:<br>
``` sudo snap install jupyter ``` <br>
``` jupyter notebook --port=<4-digit-number> ```<br>
For **<4-digit-number>**,avoid using 8888 and try using other ports.<br>
After executing these commands, you will see the following response:<br>
<img width="569" alt="image" src="https://github.com/PatrickTangwen/DSC180A-Quarter1-Integration/assets/102566928/8db3a9a6-40c0-4891-abe2-2139c7da5b14"> <br>

6. Copy the URL displayed at the bottom:<br>
For example, the URL displayed at the bootom of the screenshot is:<br>
```http://localhost:8886/?token=5d4bea140a359144f1fbe969e9251c8bc5d546329c7b46f4```
(You should have a different URL)

7. Open a new browser tab and paste the  URL into the address bar.<br>

8. Open a new terminal and navigate to the same repository directory:
   ```cd DSC180A-Quarter1-Integration```<br>
   Then, in the terminal, type the following command:
   ``` ssh -i med1.pem ubuntu@54.186.34.136 -L <4-digit-number>:localhost:<4-digit-number> ```<br>
   For **<4-digit-number>**, avoid using 8888 and try using other ports. Use the same port number as in the **step4**
   
9. Refresh the page from **step 5**, and you should now be able to access the Jupyter notebook.

## Instructions for Running the Login System Locally
### Backend
1. Open your terminal<br> 
2. Navigate to the backend directory by typing the following command:<br>
```cd login_system_backend```
3. Install the necessary dependencies:<br>
```npm install```
4. Start the backend server:<br>
```npm run dev```


### Frontend
1. Open another new terminal<br>
2. Navigate to the frontend directory by typing the following command: <br>
```cd login_system_frontend```
3. Install the required dependencies: <br>
```npm install```
4. Start the frontend server:<br>
```npm run dev```<br>
5. After starting the frontend server, you will see the URL of the local host displayed in the terminal.<br>
6. Copy and paste this URL into your web browser's address bar.<br>
7. You should now be able to access and interact with the login system locally in your browser.



