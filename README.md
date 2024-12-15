# 📱 Mobile Tag Spec Generator

The **Mobile Tag Spec Generator** is a powerful tool designed to streamline the creation of tag specifications for the **Adobe Mobile SDK**. It allows users to dynamically generate payloads for `trackAction`, `trackState`, and `Edge.sendEvent` calls. By automating the generation of both iOS Swift and Android Java/Kotlin code snippets, the tool ensures accurate and efficient implementation, testing, and debugging of tracking events.

---

## 🚀 Purpose

This tool simplifies the process of creating and validating tracking specifications for mobile applications. It provides a seamless way to configure and generate the code required to send events and data to Adobe Analytics or Adobe Experience Platform (AEP).

---

## 🛠 Features

1. **Dynamic Code Generation**:
   - Supports three key action types:
     - **`trackAction`**: Track user interactions like button clicks.
     - **`trackState`**: Track app states such as screens or pages.
     - **`Edge.sendEvent`**: Send custom XDM events to AEP.

2. **Multi-Language Support**:
   - Generates iOS Swift and Android Java/Kotlin code snippets.

3. **Key-Value Pair Customization**:
   - Allows users to define key-value pairs for tracking events.

4. **Intuitive UI**:
   - Modern, user-friendly design with copy-to-clipboard functionality.

5. **Accuracy and Efficiency**:
   - Reduces manual errors in implementation by providing pre-tested code.

---

## 🛠 Instructions for Use

1. **Select the Action Type**:
   - Choose between `trackAction`, `trackState`, or `Edge.sendEvent` using the dropdown menu.

2. **Add Key-Value Pairs**:
   - Enter the key (e.g., `page_name`) and value (e.g., `homepage`) for your event.
   - Map additional custom data points if necessary.

3. **View the Generated Code**:
   - The tool generates iOS Swift and Android Java/Kotlin code based on your inputs.

4. **Copy and Use the Code**:
   - Use the "Copy" buttons to quickly integrate the code into your mobile app.

5. **Reset or Modify**:
   - Reset the form to start over or modify the inputs to update the code dynamically.

---

## 🎯 Benefits for Stakeholders

### **Mobile Engineers**:
- **Save Time**: Automate the creation of tracking specifications.
- **Ensure Accuracy**: Generate consistent and error-free code for both iOS and Android.
- **Debugging Made Easy**: Use the tool to validate payloads and XDM objects.

### **Analysts**:
- **Better Visibility**: Preview the generated payloads and ensure they align with reporting requirements.
- **Collaboration**: Work seamlessly with engineering teams to meet data collection goals.

### **QA Testers**:
- **Validate Network Requests**: Use the generated code to validate payloads during testing.
- **Debug Faster**: Confirm that events are sent correctly to Adobe Analytics or AEP.

### **Product Managers**:
- **Streamlined Tracking**: Confirm that tracking specifications are properly implemented for key business metrics.
- **Improved Collaboration**: Ensure alignment between engineering, analytics, and QA teams.

---

## 📄 Example Outputs

### **`trackAction` Example (iOS Swift)**
```swift
let additionalData: [String: Any] = [
    "page_name": "homepage",
    "user_action": "button_click"
]
MobileCore.trackAction("button_click", data: additionalData)
