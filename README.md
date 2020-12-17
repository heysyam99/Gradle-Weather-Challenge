# Weather Challenge

> This main objective of this project is to use Gradle as a tool to forcast weather around the world by using https://openweathermap.org/forecast5 API and Gradle Http builder https://github.com/http-builder-ng/gradle-http-plugin.

## Start using the application

1. Search for a 5 days weather forecast for a specific city

`./gradlew weatherForecast -Pcity=Follow by your city name`

\*\* Quick Note

-  If your city name contain more than one words, eg Kuala Lumpur or Sao Paolo

-  Please enter your city name with string Quoatation Mark

2. Display more details about the weather forecast of the specific day

`./gradlew weatherForecast -Pcity="Kuala Lumpur -Pday=Friday`

## Problem

1. By using Open Weahter API from https://openweathermap.org/forecast5 , it will return the locale time for every 3 hours in a day. This gave us a little problem to data at 12.00 depending on request time.

## Solution

1. We will assume that we will using UTC time for every request no matter from any country around thr worlds.
