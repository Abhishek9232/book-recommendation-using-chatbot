# 📚 Book Recommendation Chatbot

An interactive chatbot that provides book recommendations based on user inputs using **IBM Watson Assistant**.  
This is a beginner-level project that integrates **IBM Cloud** services with a simple **HTML frontend**.

---

## 🌐 Technologies Used

- ✅ **HTML5** – For building the static web page
- ☁️ **IBM Cloud** – Cloud platform to host and manage services
- 🤖 **IBM Watson Assistant** – For chatbot logic and conversation flow

---

## 📄 Project Overview

This project demonstrates how to use **IBM Watson Assistant** to create a conversational chatbot for recommending books.

Users can chat with the bot, answer a few questions (like genre, interest, etc.), and receive book suggestions — all through a simple HTML interface.

---

## 📁 File Structure

```

book-recommendation-using-chatbot/
├── index.html          # Main frontend file
├── README.md           # Project documentation

````

> 💡 The actual conversation logic is handled on IBM Watson Assistant and embedded using a script or iframe into the HTML.

---

## 🚀 Getting Started

1. Clone this repository:
   ```bash
   git clone https://github.com/Abhishek9232/book-recommendation-using-chatbot.git
   cd book-recommendation-using-chatbot
````

2. Open `index.html` in any browser.

3. Ensure your IBM Watson Assistant is properly configured and integrated into the page using the script tag.

---

## 🔧 IBM Watson Assistant Setup

1. Go to [IBM Cloud Console](https://cloud.ibm.com)
2. Create a new **Watson Assistant** service
3. Design your chatbot flow (intents, entities, dialog)
4. Deploy it using the web chat integration snippet
5. Copy the integration script and paste it before `</body>` in your `index.html`

Example snippet:

```html
<script>
  window.watsonAssistantChatOptions = {
      integrationID: "your-integration-id", 
      region: "your-region", 
      serviceInstanceID: "your-service-instance-id", 
      onLoad: function(instance) { instance.render(); }
  };
  setTimeout(function(){
    const t=document.createElement('script');
    t.src="https://web-chat.global.assistant.watson.appdomain.cloud/loadWatsonAssistantChat.js";
    document.head.appendChild(t);
  });
</script>
```

---

## 💡 Future Improvements

* Add CSS styling for better UI
* Use JavaScript to handle additional logic on the frontend
* Connect Watson to a book database or API for real-time suggestions

---

## 🙋‍♂️ Author

**Abhishek Kesarwani**
🔗 GitHub: [Abhishek9232](https://github.com/Abhishek9232)

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).

