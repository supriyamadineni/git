from selenium import webdriver
from selenium.webdriver.common.by import By
from selenium.webdriver.common.keys import Keys
import time

# Start Edge
driver = webdriver.Edge()

# Open Google
driver.get("https://www.google.com")

# Find search box
search = driver.find_element(By.NAME, "q")

# Type text
search.send_keys("Hello Selenium")

# Press Enter
search.send_keys(Keys.RETURN)

time.sleep(5)

driver.quit()
Facebook
From selenium import webdriver
From selenium.webdriver.common.by import By
From selenium.webdriver.common.keys import Keys
Import time

Driver = webdriver.Chrome()

Driver.get(https://www.facebook.com)

Time.sleep(2)

Email = driver.find_element(By.ID, “email”)
Password = driver.find_element(By.ID, “pass”)

Email.send_keys(“your_email_here”)
Password.send_keys(“your_password_here”)

Password.send_keys(Keys.RETURN)

Time.sleep(5)

Driver.quit()
Elements 
From selenium import webdriver
From selenium.webdriver.common.by import By
From selenium.webdriver.common.keys import Keys
Import time

Driver = webdriver.Chrome()

Driver.get(https://www.google.com)
Time.sleep(2)

Search_box = driver.find_element(By.NAME, “q”)
Search_box.send_keys(“Selenium testing”)
Search_box.send_keys(Keys.RETURN)

Time.sleep(3)

Results = driver.find_elements(By.CSS_SELECTOR, “h3”)

For i in results[:5]:
    Print(i.text)

Driver.quit()
