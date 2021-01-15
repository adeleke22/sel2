# sel2package SelenuimTraining;

import java.util.concurrent.TimeUnit;

import org.openqa.selenium.By;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.chrome.ChromeDriver;

public class SelenuimIntro {

	public static void main(String[] args) {
	
	
		System.setProperty("webdriver.chrome.driver", "C:\\Users\\koduk\\eclipse-workspace\\Selenuim software\\chromedriver.exe");
	
		WebDriver driver = new ChromeDriver();
		
		//driver.get("https://gmail.com");
		driver.get("https://login.yahoo.com/");
		driver.manage().window().maximize();
		//driver.findElement(By.linkText("style-scope yt-button-renderer style-text size-small")).click();;
		driver.findElement(By.name("username")).sendKeys("kodukale");
		driver.manage().timeouts().implicitlyWait(10, TimeUnit.SECONDS);
		driver.findElement(By.name("signin")).click();;
		driver.findElement(By.name("password")).sendKeys("mascot0987");
		driver.findElement(By.xpath("//*[@id=\"login-signin\"]")).click();;
		driver.findElement(By.xpath("//*[@id=\"header-nav-bar\"]/li[1]/a")).click();;
		
		
		
		
		driver.manage().timeouts().implicitlyWait(10, TimeUnit.SECONDS);
		driver.findElement(By.xpath("/html/body/div/c-wiz/div[2]/div/div/div/div/div[2]/form/div/span/span")).click();
		//driver.findElement(By.xpath(null))
		
		
		
		
	}

}
