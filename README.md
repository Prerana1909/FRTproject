# FRTproject
faceauth.azurewebsites.net/docs

Face Authentication provides a variety of use cases. The primary use case is to verify same person using facial recognition or camera. API docs are present at /docs endpoint of the server.

Azure Cognitive Services
This API requires Azure Cognitive Services or Azure Face API for the face operations in the image provided. app/core/face_api.py file contains all operations used by this API such as detect, verify, createPersonGroup etc.

Azure Cognitive Services credentials are required and there is a free tier available on azure. After creating the services, create a personGroup and pass these three credentials (FACE_API_ENDPOINT, FACE_API_KEY, FACE_API_GROUP) to the server using environment variables.

export FACE_API_ENDPOINT=    # API Endpoint provided by Azure
export FACE_API_KEY=         # API Key provided by Azure
export FACE_API_GROUP=       # Created personGroup ID
