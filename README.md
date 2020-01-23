# RE
package FacebookLogin;

import org.openqa.selenium.By;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.WebElement;
import org.openqa.selenium.chrome.ChromeDriver;

public class RockInterview {

	public static void main(String[] args) throws InterruptedException {
		// TODO Auto-generated method stub

		System.setProperty("webdriver.chrome.driver", "C:\\Users\\divyasami\\Downloads\\chromedriver_win32 (1)\\chromedriver.exe");
		
		WebDriver driver= new ChromeDriver();
		
		driver.manage().window().maximize();
		
		driver.navigate().to("https://reqa.rockinterview.in/");
		
		Thread.sleep(30000);

		
		String baseUrl="https://reqa.rockinterview.in/";
		//String expectedTitle= "Rock Interview";
		
		//String actualTitle= "";
		
		driver.get(baseUrl);
		
	//	actualTitle=driver.getTitle();
		//if
			//(actualTitle.contentEquals(expectedTitle))
		    //{
			//	System.out.println("Test Passed");
			//} 
		    
		 //   else { 
		  
		  //  	System.out.println("Test Failed");
		    //}
//				driver.findElement(By.xpath("//*[@id=\"mat-dialog-0\"]/app-tour-modal/div/mat-card/div[2]/div/button[1]")).click();
				driver.findElement(By.xpath("//*[@id=\"mat-dialog-0\"]/app-tour-modal/div/mat-card/div[2]/div/button[1]")).click();
			Thread.sleep(30000);
			driver.findElement(By.xpath("//*[@id=\"mat-input-10\"]")).sendKeys("Divi");
			
			driver.findElement(By.xpath("//*[@id=\"mat-input-11\"]")).sendKeys("divya.s@rockinterview.in");
			
			driver.findElement(By.xpath("//*[@id=\"mat-dialog-1\"]/app-download-brochure/div/mat-card/form/div[2]/button")).click();
		
			Thread.sleep(30000);
			
			driver.findElement(By.xpath("/html/body/app-root/app-home/div[1]/div[1]/div/div/div[2]/ul/li[6]/a/span")).click();
			Thread.sleep(30000);
		
		//driver.findElement(By.xpath("//*[@id=\"mat-input-14\"]")).sendKeys("divya.s@rockinterview.in");
		//driver.findElement(By.xpath("//*[@id=\"mat-input-15\"]")).sendKeys("Divya@12345");
		//driver.findElement(By.xpath("/html/body/app-root/app-anonymous-layout/div/div/div/div[2]/div/app-login/div/div/div/div/form/div[2]/button")).click();
		Thread.sleep(30000);
		
		//driver.findElement(By.xpath("/html/body/app-root/app-home/div[1]/div[2]/div[4]/div[3]/div[2]/div[1]/mat-card/button")).click();
		
		driver.findElement(By.xpath("//*[@id=\"mat-input-276\"]")).sendKeys("Divya");
		
		driver.findElement(By.xpath("//*[@id=\"mat-input-277\"]")).sendKeys("Divi");
	
		driver.findElement(By.className("mat-form-field-infix")).sendKeys("RockInterview");
		
		WebElement Staffing = driver.findElement(By.xpath("//*[@id=\"mat-radio-2\"]/label/div[1]/div[1]"));
		
		WebElement Enterprise = driver.findElement(By.xpath("//*[@id=\"mat-radio-3\"]/label/div[1]/div[1]"));

		WebElement Freelancer = driver.findElement(By.xpath("//*[@id=\"mat-radio-4\"]/label/div[1]/div[1]"));
		
		Staffing.click();
		System.out.println("Staffing is Selected");
		
		Enterprise.click();
		System.out.println("Enterprise is Selected");
		
		Freelancer.click();
		System.out.println("Freelancing is Selected");
		
	//	driver.findElement(By.className("mat-button-wrapper")).click();
		
	//	driver.findElement(By.xpath("/html/body/app-root/app-anonymous-layout/div/div/div/div[2]/div[2]/app-contractors/div/div/div[1]/form/div[2]/div[2]/div[1]/div[1]/div/type-ahead/i")).click();
		//driver.findElement(By.className("ng-star-inserted")).click();
		
		//driver.findElement(By.xpath("//*[@id=\"easy-cookies-policy-main-wrapper\"]/div[2]/div")).click();
		
		//Thread.sleep(30000);
		
		//driver.findElement(By.xpath("//*[@id=\"masthead\"]/div/div/div/div[1]/div[3]/div/a")).click();
		
		//((WebElement) driver.findElements(By.xpath("//*[@id=\"ri_mobilenumber\"]"))).sendKeys("7989402217");
		Thread.sleep(20000);
			driver.quit();
			//driver.close();
		
	}

}
