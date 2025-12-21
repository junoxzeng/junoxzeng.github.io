---
layout: project
type: project
image: img/calendar1.jpg
title: "Date and Time Changer"
date: 2025
published: true
labels:
  - Java
summary: "This is an application that converts any amount of seconds to date and time"
---

<img class="img-fluid" src="clock.png">
Date and Time Converter

This project is a Java application that converts a given number of seconds into a readable date and time format. The input represents the number of seconds elapsed within a year, and the output displays the corresponding month, day, and time.

The main method for this program accepts two inputs: a seconds value and a boolean flag indicating whether the year is a leap year. The leap year flag is important because it affects the total number of seconds in the year and changes how days are distributed across months. To determine the correct date and time, the program relies on a series of arithmetic calculations and conditional checks.

This assignment was completed individually and was one of the first programming projects I worked on in my ICS 211 course. It challenged me to think carefully about time calculations, especially how leap years impact date logic. The project also served as a solid refresher on Java fundamentals and problem-solving, as I had to break down a large problem into smaller, manageable steps.

Below is a portion of the Dates class that handles the conversion logic:
```cpp
public class Dates {
	public static String computeDateTime(long seconds, boolean leapYear) {

		String[] months = {"Jan", "Feb", "Mar", "Apr", "May", "Jun",
		                   "Jul", "Aug", "Sep", "Oct", "Nov", "Dec"};

		int[] daysInMonth = {31, 28, 31, 30, 31, 30, 31, 31, 30, 31, 30, 31};
		if (leapYear) {
			daysInMonth[1] = 29;
		}

		if (seconds < 0 ||
		   (leapYear && seconds >= 31622400) ||
		   (!leapYear && seconds >= 31536000)) {
			return "illegal number of seconds";
		}

		int monthIndex = 0;
		while (seconds >= daysInMonth[monthIndex] * 86400) {
			seconds -= daysInMonth[monthIndex] * 86400;
			monthIndex++;
		}

		int day = (int)(seconds / 86400) + 1;
		seconds %= 86400;

		int hour = (int)(seconds / 3600);
		seconds %= 3600;

		int minute = (int)(seconds / 60);
		int second = (int)(seconds % 60);

		return months[monthIndex] + " " + day + " " +
		       String.format("%02d:%02d:%02d", hour, minute, second);
	}
}
