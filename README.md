# Cloud Media Streaming Platform (CAD Project)

# Phase 1: Problem Definition and Design Thinking

## Overview:

This project aims to create a virtual cinema platform using IBM Cloud Video Streaming. Users can upload and stream movies on demand, ensuring a seamless cinematic experience. The development process involves defining the platform, UI/UX design, IBM Cloud Video Streaming integration, on-demand playback, and user support.

## Implementation Stages:

1. **Platform Definition:**
   - Define architecture, choose technologies for scalability, performance, and security.

2. **UI/UX Design:**
   - Leverage UI/UX design principles for an attractive and responsive interface.

3. **IBM Cloud Video Streaming Integration:**
   - Configure and integrate IBM Cloud Video Streaming services, ensuring secure access.

4. **On-Demand Video Playback:**
   - Design user-friendly playback system utilizing IBM Cloud capabilities.

5. **User Support:**
   - Establish user support channels, gather feedback for continuous improvement.

## Features:

### 1. User Registration:
   - Sign-up/login via email or Google.
   - Profile management with authentication mechanisms.

### 2. Video Upload:
   - Upload videos with metadata (title, description, genre) and customizable thumbnails.

### 3. On-Demand Streaming:
   - Powerful search with auto-suggestions.
   - High-quality playback with standard controls.

### 4. UI/UX Design Principles:
   - Prioritize simplicity and responsiveness.
   - Use intuitive icons for essential actions.

### 5. Video Upload Process:
   - Efficient file selection and upload.
   - Metadata management with edit options.

### 6. Streaming Integration:
   - Configure IBM Cloud for reliable storage and streaming.
   - Implement a seamless video player for high-quality playback.

### 7. User Experience:
   - Social engagement features (likes, comments, sharing).
   - User ratings, reviews, and personalized recommendations.

## Usage:

1. Clone the repository.
2. Follow installation instructions in the 'Installation.md' file.
3. Run the platform on your local environment.

## Feedback:

Your feedback is crucial for continuous improvement. Reach out through our support channels or email for assistance.

---

# Phase 2: Innovation
## Introduction:
Transform the proposed approach into an innovative Cloud Media Streaming Platform through development, testing, and deployment. Incorporate user-generated playlists and real-time chat for an enhanced movie-watching experience.

## Innovative Solutions:
### User-Generated Playlists:

#### Development Steps:
Utilize frontend components (UI, Drag & Drop, Preview) for playlist creation.
Implement backend services (Database, APIs for CRUD, Authentication) for playlist management.
Enable real-time collaborative playlist editing using technologies like Socket.io.
### Real-Time Chat:

#### Development Steps:
Create a real-time chat interface using an SDK for one-on-one and group chat.
Implement chat rooms for different user groups and communities.
Integrate moderation tools (Content Moderation API, Reporting, Administrator dashboard) to ensure a positive chat environment.
### Implementation Strategy:
Integrate innovative solutions thoughtfully, aligning with design thinking principles. Consider specific algorithms based on streaming service needs and available technology.

### Adaptive Streaming:
Commonly, employ adaptive streaming algorithms like HLS or DASH, dynamically adjusting video quality based on the viewer's internet connection and device capabilities.

### IBM Cloud Video Streaming:
Utilize IBM Cloud Video Streaming for features like content protection, analytics, and seamless integration with other IBM Cloud services. Refer to IBM's documentation or contact support for detailed information.

---

# Phase 3: Development Part 1
## Introduction:
Building a virtual cinema platform using IBM Cloud Video Streaming involves several steps. This phase focuses on Platform Definition, User Interface Design, and User Registration/Authenticate.

## Development Environment:
Backend: Python and Flask
Frontend: HTML, CSS
Client-side interactions: JavaScript
## Platform Features:
### User Registration and Authentication:

Handled using IBM Cloud Video Streaming credentials.
Optionally integrated with a user authentication system.
### Video Streaming and Management:

Supports live streaming and on-demand playback.
Allows editing of video metadata (title, description, thumbnail).
### Real-Time Chat:

Integrated chat for user discussions during video watching.
### On-Demand Playback:

Viewers can pause, play, fast-forward, rewind, and re-watch on demand.
### User Feedback:

Provides feedback messages for actions or errors.
## Intuitive UI Design:
Design principles focus on simplicity and user-friendly navigation. Key pages include:

Home Page: Navigation links, video thumbnails.
Video Playback Page: Player with controls, real-time chat.
User Profile Page: User stats, playlists.
Upload Video Page: File upload with title, description, thumbnail.
Playlist Page: Add, view, or manage videos in playlists.
## Implementation:
HTML and CSS used for key pages. Design prioritizes responsive layout and intuitive controls for a seamless user experience.

## User Registration and Authentication:
Common procedures involve:

Package installation for Flask application.
Flask app configuration with secret key and database setup.
User model definition in Python.
Creation of registration and login forms.
User registration route implementation.
User login route setup.
User logout route creation.
Application execution using the Flask run command.
By following these steps, users can register, log in, and log out seamlessly. Customize routes and features based on specific application requirements.

---

# Phase 4: Development Part 2
## Introduction:
Continuing the development of the virtual cinema platform involves integrating video streaming services and enabling on-demand playback. This phase utilizes Flask and HTML for implementation.

## Steps:
### Environment Setup:

Ensure Python and pip are installed.
Create and activate a virtual environment.
### Install Dependencies:

pip install Flask Flask-WTF Flask-Login Flask-SocketIO
### Create Flask App:

Set up a basic Flask app with a secret key and SocketIO support.
### Define Video Model:

Utilize Flask-SQLAlchemy to define the Video model.
### Create Video Upload Form:

Implement a form for video uploads using Flask-WTF.
### Implement Video Upload Route:

Create a route for handling video uploads.
### Implement Video Streaming Route:

Develop a route for on-demand video playback.
### Create Video Streaming HTML Template:

Design a template for video playback with a video player.
### Run the Application:

flask run
### Integrating IBM Cloud Video Streaming:

Set up an IBM Cloud account.
Create a streaming channel.
Obtain API key and access token.
Configure the application for IBM Cloud Video Streaming.
Bind IBM Cloud Video Service to the Cloud Foundry App.
### Deployment using Docker and Cloud Foundry:

Create a Flask application interacting with the IBM Cloud Video Streaming API.
Build a Docker image and push it to a container registry.
Deploy the application to Cloud Foundry.
### Restage Your Cloud Foundry App:

cf restage YOUR_APP_NAME
### Access Your Cloud Foundry Application:

Open the assigned URL in your web browser.
## IBM Cloud Foundry Deprecation:
IBM Cloud Foundry is deprecated and will be disabled on June 1, 2023. Users are advised to migrate to alternative IBM Cloud compute services:

IBM Cloud Code Engine (serverless platform).
IBM Cloud Kubernetes Service (containerized workloads).
Red Hat OpenShift on IBM Cloud (Kubernetes container platform).
## Migration Checklist:
### Investigate & Review:

Review current IBM Cloud Foundry application deployments.
### Choose Compute Service:

Investigate suitable IBM Cloud compute services.
### Deploy Application:

Deploy your application to the chosen IBM Cloud compute service.
### Balance Traffic:

Distribute incoming traffic between IBM Cloud compute types.
### Shutdown Cloud Foundry Apps:

Shut down IBM Cloud Foundry applications.

Follow the migration checklist for a smooth transition. Regularly update your application based on user feedback and evolving requirements. Ensure secure handling of sensitive information and refer to official documentation for detailed information and updates.
