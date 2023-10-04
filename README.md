# Emmet Browser
![image](https://github.com/Angad-Godara/emmet-browser/assets/104693483/90d67855-fcc0-4753-99a3-b7a2dca1e777)<br/>
## Introducing Emmet Browser: Your Secure & Fast Browser

Emmet is a custom web browser designed exclusively for the Indian market. It combines the power of the Chromium engine with a unique feature – built-in CCA India root certificate, ensuring a seamless and secure browsing experience for Indian users. With Emmet, you can surf the web confidently, knowing your online activities are protected by the highest standards of security and performance, tailored to meet the specific needs of Indian internet users.


## 🖥️ Tech Stack

**Existing libraries that may be used in the browser development process are:**

**Chromium/Blink:**
   - Chromium is the open-source project behind Google Chrome, providing a comprehensive web browser framework.
   - Blink is the rendering engine within Chromium responsible for parsing and rendering web content.
   - Leveraging Chromium/Blink provides access to a powerful, widely-used rendering engine with excellent standards support.

**Electron:**
   - Electron is a cross-platform framework that enables the creation of desktop applications using web technologies.
   - It allows developers to build standalone browser applications by combining Chromium with Node.js.
   - Electron simplifies the process of packaging web content into desktop applications.

**WebKit:**
   - WebKit is an open-source web rendering engine used in browsers like Safari.
   - It offers a versatile framework for rendering web content, including HTML, CSS, and JavaScript.
   - Developers can use WebKit to create custom web browsers or embed web content in applications.

**CEF (Chromium Embedded Framework):**
   - CEF enables the integration of a Chromium-based web browser within desktop applications.
   - It offers a C/C++ API for embedding a web browser component into software applications, making it suitable for creating custom browser interfaces.

**React and React Native:**
   - React is a JavaScript library for building user interfaces, and React Native extends this capability to mobile platforms.
   - These libraries can be employed for creating the user interface of the browser, including tabs, menus, and toolbar components.

**Node.js:**
   - While Node.js is mainly associated with server-side development, it can also be used for browser-related tools and extensions.
   -Node.js can be used as the backend of the custom browser such as managing bookmarks, history, downloads, and extensions.

**WebExtensions API:**
   - The WebExtensions API is a standardized interface supported by multiple browsers like Firefox and Chrome.
   - It simplifies the development of browser extensions that work across different browsers.
   - Developers can use it to create add-ons and extensions with consistent APIs.

**Lighthouse:**
   - Lighthouse is an open-source tool from Google designed for auditing web pages.
   - It assesses various aspects of web pages, including performance, accessibility, and best practices.
   - Developers can integrate Lighthouse into the development process to ensure web standards compliance.
   - 
**Selenium:**
 - Selenium is a popular testing framework used for automating web browser interactions.
 - It provides support for multiple programming languages and browsers, making it suitable for cross-browser testing.



   

## 🚀Significant enhancements to be made in the core engine


Major drawbacks existing in the Chromium engine and their solution are:

1\.**Privacy Concerns:**

*Chromium based browser face criticism for their data collection practices and perceived lack of privacy*. 

We will optimize privacy settings, including options to disable data collection features. Inform users about privacy-related choices during the initial setup. Consider forking Chromium to create a privacy-focused browser with stricter default privacy settings.

- **History:** Browsing activity done in standard mode to be recorded in reverse chronological order, with the option for user to clear them.
- **Phishing Protection:** The browser should force for HTTPS and should include malicious content blockers by avoiding unnecessary pop-ups.
- **Download Management:** Option to access the downloaded content for offline browsing.

**2.Secure Web Connections:**

Integrate security features, including the management of root certificates. For the CCA India root certificate, we will need to include it in the browser's certificate store.

- **Trust Store:** Service to indicate trust (Preloaded with CCA India Root Certificate) of websites.
- **Web3 support:** Browser enables support for Web3 content.


3\.**High Resource Usage:**

*To tackle high memory and CPU usage in Chromium-based browsers,* we will optimize memory management, introduce tab suspension for inactive tabs (**lazy tab loading**), and provide customizable resource management settings to boost system performance and preserve battery life.

**4.Resource Intensive Updates:**

Chromium updates can be resource-intensive and disrupt user workflows.

We will implement background updates that do not require a browser restart, reducing the impact on users. Allow users to schedule updates to occur during low-activity periods.

- **Browser Extension:** Browser should support enabling/disabling extensions.

**5.Limited Support for Older Hardware/ Compatibility Issue:**

` `As Chromium evolves, it may not perform well on older or low-end hardware.

We will create a lightweight version or mode of the browser optimized for older hardware. Prioritize performance optimizations for resource-constrained devices.

- **Speed and Memory Management:** The browser should use minimal CPU and have minimal possible memory footprint.
- **Seamless Browser Update Mechanisms:** Support Auto-update and prompting for Updates.

**6.Heavy Dependency on Google Services**

*Chromium is developed by Google and has strong ties to Google services, which may not align with the goals of privacy-focused browsers.*

-We will Fork Chromium to create a custom build that reduces dependencies on Google services. Implement alternative sync mechanisms for bookmarks, passwords, and other user data.

- **Multiple Search Engine options:** Support for multiple search engines for user to select from.

6\.**Limited Customization**

Chromium browsers tend to limit the extent to which users can customize the user interface and behavior.

We will provide browser extensions and themes that allow users to customize the browser to their liking. Consider building a user-friendly interface for advanced customization options without overwhelming less tech-savvy users.

- **Customizable Visual Appearance:** Enable users to have their preferences.
- **Bookmark management:** Allows user to add & remove bookmarked websites for frequent access.


## 🚀Challenges and limitations that we foresee in the development of the proposed web browser

1\. **Compatibility and Standards Compliance:**

**Challenge:** Ensuring compatibility with the ever-evolving web standards and rendering engine updates can be challenging.

**Solution:** Regularly update the browser's rendering engine (e.g., Blink, WebKit) and conduct thorough compatibility testing.

2\. **Security and Privacy:**

**Challenge:** Protecting users from security threats, including malware, phishing, and data breaches, is a top priority.

**Solution:** Implement robust security measures, such as sandboxing, strict content security policies, and regular security audits. Educate users on safe browsing practices.

3\. **Performance Optimization:**

**Challenges:** Maintaining a fast and responsive browser, especially when handling resource-intensive websites and web applications.

**Solution:** Continuously optimize the browser's rendering engine, improve memory management, and leverage hardware acceleration. Implement performance profiling tools for developers to identify bottlenecks.

4\. **User Interface Design:**

**Challenge:** Creating a user-friendly and intuitive interface that caters to a diverse user base.

**Solution:** Invest in user interface design, conduct usability testing, and provide customization options. Listen to user feedback to make iterative improvements.

5\. **Cross-Platform Compatibility:**

**Challenge:** Ensuring the browser functions seamlessly on various operating systems and devices.

**Solution:** Use cross-platform development frameworks like Electron or QtWebEngine. Extensively test and adapt the user interface for different platforms.

7\. **Resource Consumption:**

**Challenge:** Web browsers often consume significant system resources, affecting device performance.

**Solution:** Implement resource management strategies, like **lazy tab loading** and efficient memory usage. Offer settings to control resource consumption.

8\. **Accessibility:**

**Challenge:** Ensuring that the browser is accessible to users with disabilities, complying with accessibility standards.

**Solution:** Implement accessibility features, such as support for screen readers and keyboard navigation. Regularly test with users who have disabilities and adhere to WCAG guidelines.


10\. Competition:

**Challenge:** The web browser market is highly competitive, with well-established players.

**Solution:** We will differentiate our browser through unique features, performance improvements, and a strong focus on security and privacy. We aim to build a passionate user community and engage with user feedback.

12\. User Data Handling:

**Challenge:** Handling user data responsibly and respecting privacy preferences.

**Solution:** Implement clear data handling policies, offer robust privacy settings, and provide users with control over their data. Comply with data protection regulations like GDPR.









© 2023 Team Emmet

