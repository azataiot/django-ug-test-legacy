# Django Test App for Uyghur (ug)

This is a test app for Django. It is a simple poll app based on Django's official tutorial [Writing your first Django app](https://docs.djangoproject.com/en/4.2/intro/tutorial01/). The primary purpose of this app is to test and demonstrate the Uyghur (ug) translation support added to Django.

## Using the Sample Application

The repository comes bundled with a sample Django application that's already configured to use the Uyghur language. Here's how you can run and test it:

### Setup:

1. **Clone the Repository:**

   First, clone the repository to your local machine.

   ```bash
   git clone https://github.com/azataiot/django-ug-test.git
   cd fork-django
   ```

2. **(Optional but Recommended) Create a Virtual Environment:**

   This step ensures that the custom Django version and other dependencies don't interfere with other projects or system-wide installations.

   ```bash
   python -m venv myenv
   source myenv/bin/activate  # On Windows use: myenv\Scripts\activate
   ```

3. **Install Dependencies:**

   If the repository has a `requirements.txt` file (or similar), install the required packages.

   ```bash
   pip install -r requirements.txt
   ```

   If not, follow the earlier provided steps to install the custom Django version.

4. **Navigate to the Sample Application Directory:**

   ```bash
   cd django-ug-test
   ```
   
5. **Run Migrations (if required):**

   ```bash
   python manage.py migrate
   ```

6. **Start the Development Server:**

   ```bash
   python manage.py runserver
   ```

   This will start the server, and you can visit `http://127.0.0.1:8000/` in your browser to access the application.

### Exploring the Sample Application:

With the server running, you can explore various parts of the application to see the Uyghur language in action (Check the Django Admin for example). If the sample application has specific features or sections that demonstrate the Uyghur language more prominently, navigate to those parts.

---

Remember: This is a sample application meant for testing purposes. It's recommended not to use it in a production environment.

## Installation for a fresh Django Project

As of now, Django 5.0 has not been officially released, and the Uyghur translation is expected to be included in this version. Therefore, to test the Uyghur support, you'll need to install our custom Django version from the GitHub repository.

### Steps:

1. **(Optional but Recommended) Create a Virtual Environment:**

   This step ensures that the custom Django version doesn't interfere with other projects or system-wide installations.

   ```bash
   python3 -m venv myenv
   source myenv/bin/activate  # On Windows use: myenv\Scripts\activate
   ```

2. **Install the Custom Django Version:**

   Use pip to install Django directly from the specific branch of the repository where Uyghur support has been added.

   ```bash
   pip install git+https://github.com/azataiot/django.git@dev#egg=django
   ```

3. **Verify the Installation:**

   After installation, you can check the Django version to confirm that the correct version is being used.

   ```bash
   python -c "import django; print(django.get_version())"
   ```

   This command should display the version of Django from the `dev` branch of the `fork-django` repository. If modifications were made to the version, it should reflect those changes.

### Proceed with Django Project:

Once the custom Django version is installed, you can use Django commands such as `django-admin startproject myproject` to create new projects. Navigate to the `myproject` directory and use the `runserver` command to start the development server. You can then explore and test the Uyghur language support in your projects.

---

Note: Always remember that this is a custom version of Django and may contain changes that are not in the official Django release. It is recommended not to use this version for production applications until the official Django team reviews and potentially merges the related PR.
