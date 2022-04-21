# Projects

A project is the container for developing dialogs. Projects can contain individual dialogs, or they can contain multiple dialogs to form a more fully functioning bot. The project is allocated a capacity for runtime and has its own API endpoint for interaction. Projects can be imported and exported through the UI and so can be version controled or promoted through a dev - test - production pipeline.

## Create a Project 
The new project button on the main project dashboard view is used to create a new project. Give the project a name (no spaces), a description, and a Default Language (we currently support English, French, or German) then hit create.
Image Here

## Project Details - Home
The Home section of the Project Details displays information about the project, including the project name, the description, the project id (used in the API URL), and language). This section also displays project status information like the number of intents and dialogs in the project, the users role and the training status. 