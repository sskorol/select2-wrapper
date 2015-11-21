# Selenium Select2 wrapper

Allows WebDriver to interact with Select2 via its native API.

You can find more details in the following article:
 
```java
	@HTML(searchBy = CSS_SELECTOR, value = "div[id*=listBox1]")
	private Select2 listBoxWeekDay;

	public HomePage selectWeekDay(final String day) {
		listBoxWeekDay.selectByVisibleText(day);
		return this;
	}

	public String getSelectedWeekDay() {
		return listBoxWeekDay.getSelectedText();
	}
```