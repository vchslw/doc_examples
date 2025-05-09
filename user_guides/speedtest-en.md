---
description: >-
  User guide for Speedtest service. The target audience is people with limited
  technical skills.
---

# Speedtest (English)

## About Speedtest service

Speedtest is an online tool that evaluates the speed and quality of your Internet connection.

You simply select the test parameters, run the test, wait for it to finish, and then view the results. You can save the results as a link and share it on social media and messaging apps.

## How to check Internet speed and quality on your device

1. Go to the [Speedtest website](https://speedtest.rt.ru/).
2. The opened page will automatically run the test.

{% hint style="info" %}
In most cases, the automatically run test gives results that do not correspond to the real values for the following reasons:

* As the target server selected a server providing the fastest and highest quality connection.

<details>

<summary>What is a target server?</summary>

The Internet consists of many servers (computers) connected to each other. The servers communicate with each other by sending data packets — some data that servers send and receive.

When you go online (for example, open any website), your device connects to the server that hosts this website. So, this is a target server — the server your device is communicating with.

</details>

* The test is executed in a [single-threaded mode](speedtest-english.md#what-are-threads-and-which-packet-sending-mode-should-be-selected).
* Only one test is performed.

If this test is sufficient for you, wait until the test is completed and then view the [results](speedtest-english.md#performing-results).

If you need to get results close to the real values, follow the next steps of this guide.
{% endhint %}

3. Click **Break**.
4. Select the city where the target server is based (only some big cities of Russian Federation are available for selection):

* From the list: Click the down arrow next to the city name on the right side of the screen to expand the list, then select the city from the list.
* Search: Click the down arrow next to the city name on the right side of the screen. In the **Find city** input, enter the name of the city and tap it when it appears on the screen.
* On the map: Scroll down the page, click **Select a server on map**, and pick the city.

5. Select the testing mode:

* **Basic**: This mode is designed for performing a single test.
* **Advanced**: This mode allows you to run several tests with a specified interval between them.

{% hint style="info" %}
Internet connection speed and quality are subject to change. So, performing multiple tests with an interval between them can provide more accurate results.
{% endhint %}

6. If you have selected **Advanced mode**, please specify the settings:

* **Number of tests** to be performed.
* **Interval in minutes**: This is a period between tests.

{% hint style="info" %}
The more both values are increased, the more accurate results you will get.
{% endhint %}

7. Select the packets sending mode:

* **Single-threaded**: Only one data stream will be used. This is suitable for testing a single channel and getting a general idea of the speed and quality of the connection.
* **Multithreaded**: Multiple streams are used simultaneously for testing. This mode allows you to find out how the Internet works under real-world usage conditions.

<details>

<summary>What are threads and which packets sending mode should be selected?</summary>

A data stream is a channel by which your device exchanges data with the server.

For example, consider three applications on your laptop that are currently using Internet connection:

* A browser with two tabs open, one with a video enabled and the another with an opened online shop.
* Messenger.
* Weather app.

In this case, four streams will be active:

* To play the video on the first tab.
* To interact with the online shop on the second tab.
* To send and receive messages in the messenger.
* To update the weather data.

**Multithreaded** mode reflects real-world usage conditions, as multiple applications often run simultaneously on the same device and use the Internet.

**Single-threaded** mode is an ideal fit to estimate the single stream speed when only one channel is used. For example, for a specific application like messenger or for watching video.

</details>

8. Click **Start**.

{% hint style="warning" %}
Please note that it is impossible to change test settings or view all performance results while the test is running.
{% endhint %}

9. Wait for the test to complete. Then the test results will be displayed on the screen.
10. Proceed to view the results.

## Performance results

Once the tests are completed, the screen displays the values of four parameters from the last test:

* **Download**: The speed of downloading data from the Internet to your device, measured in Mbps. A higher download speed means faster page loading, file downloading, and video playback.
* **Upload**: The speed of sending data to the Internet from your device, measured in Mbps. For example, when sending an email, making a call, or sharing a screen. A higher value accelerates the upload of data and files.
* **Ping** is the time it takes to send a small data packet from your device to a server and receive the data packet as response, measured in ms. High ping values can result in service crashes or delays.
* **Jitter**, measured in ms, indicates the variability in data packets delivery time. A high jitter value can cause connection failures in latency-sensitive applications, such as video calling or online gaming.

Examples of good, normal, and bad values for each parameter can be found [here](speedtest-english.md#performing-results).

### Graphical results from multiple tests

The results of several tests are displayed on a graph below the last test. This graph shows the parameters obtained from all the tests performed in **Advanced mode**.

By clicking on the parameter name below the graph, you can disable the display of any parameter on the graph.

If tests were performed on a computer, you can view each parameter separately. To do so, hover over the name of the parameter you would like to view.

### Results from last 10 tests

To view the results of the last 10 tests, click **Results**. A page with a graph and a table of the performed tests will open.

To view the results of a single test, click its **Testing time** in the table. This will open a page with the results of this test.

### Examples of test result values

Here are examples of good, normal, and bad values for home and mobile Internet:

{% tabs %}
{% tab title="Home Internet" %}
| Parameter and its unit of measure | Good value    | Normal value | Bad value    |
| --------------------------------- | ------------- | ------------ | ------------ |
| Download, Mbps                    | 100 and above | 25–100       | Less than 25 |
| Upload, Mbps                      | 20 and above  | 5–20         | Less than 5  |
| Ping, ms                          | Less than 10  | 10–30        | 30 and above |
| Jitter, ms                        | Less than 1   | 1–10         | 10 and above |
{% endtab %}

{% tab title="Mobile Internet" %}
| Parameter and its unit of measure | Good value   | Normal value | Bad value    |
| --------------------------------- | ------------ | ------------ | ------------ |
| Download, Mbps                    | 50 and above | 10–50        | Less than 10 |
| Upload, Mbps                      | 20 and above | 5–20         | Less than 5  |
| Ping, ms                          | 10–20        | 20–50        | 50 and above |
| Jitter, ms                        | Less than 5  | 5–20         | 20 and above |
{% endtab %}
{% endtabs %}

### How to save and export test results

Upon completion of each test, a unique link to the results is automatically generated. This link can be saved by copying and pasting it into a document in any text editor. It can also be shared via the following services:

* Telegram.
* VKontakte.
* WhatsApp.
* Odnoklassniki.
* Email.

To share the link, click the service icon and select the recipient in the opened application.
