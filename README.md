# ValtechPro1
ValtechPagesFunctionality 1


package ValtechPagesFunctionality;

import org.junit.Assert;
import org.openqa.selenium.By;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.chrome.ChromeDriver;

public class ValtechFunctionalTesting {

	public static void main(String[] args) {
		// TODO Auto-generated method stub

		System.setProperty("webdriver.chrome.driver", "C:\\Users\\user\\Downloads\\chromedriver_win32\\chromedriver.exe");
		
		WebDriver driver = new ChromeDriver();
		
		driver.get("https://www.valtech.com/");  
		
		driver.manage().window().maximize();
		
		Assert.assertTrue(true);   
		
		driver.findElement(By.cssSelector("#navigationMenuWrapper > div > ul > li:nth-child(1) > a")).click();
		
		driver.findElement(By.cssSelector("#navigationMenuWrapper > div > ul > li:nth-child(3) > a")).click();
		
		driver.findElement(By.cssSelector("#navigationMenuWrapper > div > ul > li:nth-child(2) > a")).click();
		
		driver.findElement(By.cssSelector("#CTA-form-trigger > div > div > span")).click();
		
	}
	
}
