# **Blog Project**

Welcome to the Blog project! This web application allows you to create and share interesting blog posts with others. You can tag your posts, enable commenting, and even share your favorite blogs via email. The project is built using Django 4 and uses PostgreSQL as the database, which can be easily set up with Docker Compose.

## **Getting Started**

### **Prerequisites**

Make sure you have the following installed before starting:

- [Python](https://www.python.org/downloads/) (3.8 or higher)
- [Docker](https://www.docker.com/get-started)
- [Docker Compose](https://docs.docker.com/compose/install/)
- [Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)

### **Installation Steps**

1. Clone the repository:
    
    ```bash
    git clone https://github.com/OrenRenner/blog_project.git
    ```
    
2. Change into the project directory:
    
    ```bash
    cd blog_project
    ```
    
3. Create and activate a virtual environment:
    
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```
    
4. Install dependencies:
    
    ```bash
    pip install -r requirements.txt
    ```
    
5. Start the PostgreSQL database using Docker Compose:
    
    ```bash
    docker-compose up -d
    ```
    
6. Apply migrations to create the database schema:
    
    ```bash
    python manage.py migrate
    ```
    
7. Create a superuser for the admin panel:
    
    ```bash
    python manage.py createsuperuser
    ```
    
8. Start the Django development server:
    
    ```bash
    python manage.py runserver
    ```
    
9. Open your browser and go to http://127.0.0.1:8000/admin/ to log in with the superuser credentials and add some blogs.
10. Visit http://127.0.0.1:8000/ to view the blog posts.

## **Features**

- **Blog Feed:** Explore a feed of interesting blog posts.
- **Tagging:** Categorize your blogs by adding tags.
- **Commenting:** Engage with other users by leaving comments on their posts.
- **Email Sharing:** Share your favorite blogs with friends via email.

## **Contributing**

We welcome contributions! If you find a bug or have an enhancement in mind, please open an issue or submit a pull request.

Happy blogging! 🚀
