<p align="center">
  <a href="https://discord.gg/your-invite-link">
    <img src="https://img.shields.io/discord/1236779067252936736?color=7289DA&label=Discord&logo=discord&logoColor=white&style=for-the-badge" alt="Discord">
  </a>
</p>

**This project is currently in early development, and things may break unexpectedly.**

# Briefbox

Briefbox is a tool for archiving emails from multiple IMAP and POP3 accounts. It provides a user-friendly web interface for managing email accounts, searching archived emails, and viewing email details along with attachments. One of the standout features of Briefbox is its advanced search functionality, which allows users to quickly find specific emails using various criteria.

<table>
  <tr>
    <td><img width="500" alt="image" src="https://github.com/bandundu/email-archiver/assets/41874924/c6775f3b-f1b8-41e5-9650-0278fd30a813"></td>
    <td><img width="500" alt="image" src="https://github.com/bandundu/email-archiver/assets/41874924/dcd67645-f809-45cc-8f01-b3574df20bbe"></td>
  </tr>
  <tr>
    <td><img width="500" alt="image" src="https://github.com/bandundu/email-archiver/assets/41874924/c8ff9719-3798-4ee8-a2ca-ac6992c6fca2"></td>
    <td><img width="500" alt="image" src="https://github.com/bandundu/email-archiver/assets/41874924/cabdef22-4f56-47e7-ace3-07c39e8416fc"></td>
  </tr>
</table>







## Prerequisites

- Python 3.x
- Node.js
- npm

## Setup and Usage

1. Clone the repository:

   ```bash
   git clone https://github.com/bandundu/email-archiver.git
   ```

2. Navigate to the backend directory:

   ```bash
   cd email-archiver/backend
   ```

3. Create a virtual environment:

   ```bash
   python -m venv .venv
   ```

4. Activate the virtual environment:

   ```bash
   source .venv/bin/activate
   ```

5. Install the required dependencies:

   ```bash
   pip install -r requirements.txt
   ```

6. Launch the backend:

   ```bash
   python app.py
   ```

   The backend will start running on `http://localhost:5050`.

7. Open a new terminal and navigate to the frontend directory:

   ```bash
   cd ../frontend/briefbox-front
   ```

8. Install the frontend dependencies:

   ```bash
   npm install
   ```

9. Start the frontend development server:

   ```bash
   npm start
   ```

   The frontend will be accessible at `http://localhost:3000`.

10. Access the web interface by opening a web browser and navigating to `http://localhost:3000`.

11. Use the web interface to add email accounts, search for emails, and view email details.

**Note:** I apologize for the inconvenience, but I am are currently working on improving the Docker Compose setup for a smoother deployment experience. In the meantime, please follow the above steps for a bare-metal installation.

<!-- 1. Create a `docker-compose.yml` file in a folder of your chosing with the following content:

```yaml
version: '3'

services:
  backend:
    # latest-arm for ARM devices like Raspberry Pi
    image: bandundu/briefbox-backend:latest
    ports:
      - "5050:5050"
    volumes:
      - ./:/app/data
    environment:
      - FLASK_ENV=development
      - FLASK_APP=app.py

  frontend:
    # latest-arm for ARM devices like Raspberry Pi
    image: bandundu/briefbox-frontend:latest
    ports:
      - "3000:3000"
    depends_on:
      - backend
```

> **Note:** For ARM devices like Raspberry Pi, use the `latest-arm` tag for both backend and frontend images.

2. Run the following command to start the containers:

```bash
docker-compose up
```

3. Access the web interface by opening a web browser and navigating to `http://localhost:3000`.

4. Use the web interface to add email accounts, search for emails, and view email details. -->

## Star History

[![Star History Chart](https://api.star-history.com/svg?repos=bandundu/email-archiver&type=Date)](https://star-history.com/#bandundu/email-archiver&Date)
