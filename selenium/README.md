# Selenium

Selenium is a open-source framework and a suite of tools designed for automating web browsers. It allows you to control a web browser programmatically, perform various tasks on web applications, and automate the testing of web application.

Selenium is commonly used for web testing but can also be used for web scraping, data extraction, and automating repetitive tasks involving web browsers.



The core component of Selenium is the WebDriver, which acts as a bridge between your code and web browser.

You can use WebDriver to simulate user interactions like clicking buttons, filling forms, navigating between pages, and extracting data from web pages.



## Locating Elements

- by **Id**

  ```python
  login_form = driver.find_element(By.ID, "loginForm")
  ```

  - Use this when you know the ***id*** attribute of element/tag.
  - First element with matching ***id*** attribute will be return.
  - If no element has matching ***id*** attribute, a **NoSuchElementException** will be raised.

- by **Name**

  ```python
  username = driver.find_element(By.NAME, 'username')
  password = driver.find_element(By.NAME, 'password')
  ```

  - Use this when you know the ***name*** attribute of element/tag.
  - First element with matching ***name*** attribute will be return.
  - If no element has matching ***name*** attribute, a **NoSuchElementException** will be raised.

- by **Xpath**

- Hyperlinks by **Link Text**

- Elements by **Tag Name**

- Elements by **Class Name**

- Elements by **CSS Selector**
