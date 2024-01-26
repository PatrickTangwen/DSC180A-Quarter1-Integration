# DSC180A-Quarter1-Integration

## Instructions for accessing AWS on a local machine.

1. Open terminal and clone this repository using the following command: <br>
```git clone https://github.com/PatrickTangwen/DSC180A-Quarter1-Integration.git```

3. Navigate to the repository directory: <br>
```cd DSC180A-Quarter1-Integration```<br>

4. Use the following commands to gain access to the AWS server:<br>
``` chmod 0400 med1.pem ``` <br>
``` ssh -i med_dash.pem ubuntu@54.214.106.120 -L xxxx:localhost:xxxx ``` <br>
(Make sure the file name is **"med1.pem"** with **"pem"** extension instead of other file extension)<br>
You should replace **xxxx** by **<any 4-digit-number>** to avoid using the same port number.

5. In the same terminal, use the following commands to connect to the Jupyter notebook:<br>
``` source venv/bin/activate ``` <br>
``` jupyter notebook --port=<same 4-digit-number you have placed above> ```<br>
After executing these commands, you will see the following response:<br>
<img width="566" alt="image" src="https://github.com/PatrickTangwen/DSC180A-Quarter1-Integration/assets/102566928/7aa23c32-c9cb-4452-ba0d-57b3b6627957"> <br>

6. Copy the URL displayed at the bottom:<br>
For example, the URL displayed at the bootom of the screenshot is:<br>
```http://localhost:1112/lab?token=3dfe77414fa7c9d8683eb806ff737a8d89eac2c78b1659fc``` <br>
(You should have a different URL as you use different port number)

7. Open a new browser tab and paste the URL into the address bar, and you should now be able to access the Jupyter notebook.<br>
   

## Instructions for Running the Login System Locally
If you haven't install Node.js in your computer,please download it from the following url:<br>
[Node.js](https://nodejs.org/en/download)

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



