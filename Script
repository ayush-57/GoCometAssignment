
import java.io.*;
import org.junit.Assert; 
import org.openqa.selenium.By;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.WebElement;
import org.openqa.selenium.chrome.ChromeDriver;
import io.github.bonigarcia.wdm.WebDriverManager;

public class AssignmentScript {

	public static void main(String[] args){

		WebDriverManager.chromedriver().setup();
		WebDriver driver=new ChromeDriver();
		String URL="https://www.demoblaze.com/index.html";
  
		// Open URL and Maximize browser window
		driver.get(URL);
		driver.manage().window().maximize();

		//Click on a product
		driver.findElement(By.linkText("Samsung galaxy s6")).click();
		String product = driver.findElement(By.linkText("Samsung galaxy s6")).getText();
		//Click on add to cart
		driver.findElement(By.linkText("Add to cart")).click();
		//Clicking on cart
		driver.findElement(By.linkText("Cart")).click();
		String CartProduct = driver.findElement(By.linkText("Samsung galaxy s6")).getText();
  
		//comparing both product titles
		Assert.assertEquals(product, CartProduct);
		System.out.println("Product is present in cart");
	}
}
