# badminton-booking.github.io-
# 🏸 Badminton Court Booking Management System

A complete automation solution for managing badminton court bookings using Google Sheets, featuring both a web form interface and an unofficial WhatsApp bot for seamless booking management.

## 📋 Overview

This project provides two complementary solutions for automating badminton court bookings:

1. **🌐 Web Form Solution** - A beautiful, responsive web form that directly updates Google Sheets
2. **🤖 WhatsApp Bot Solution** - An unofficial bot that monitors WhatsApp group messages and automatically updates bookings

## ✨ Features

### Web Form Solution
- ✅ Modern, responsive design with gradient styling
- ✅ Direct Google Sheets integration via Google Apps Script
- ✅ Real-time form validation and error handling
- ✅ Mobile-friendly interface
- ✅ Automatic date validation (prevents past dates)
- ✅ Loading states and success/error feedback
- ✅ Free to deploy and maintain

### WhatsApp Bot Solution
- ✅ Automatic message monitoring in WhatsApp groups
- ✅ Smart message parsing for booking requests
- ✅ Holiday/skip day command support
- ✅ Automatic Google Sheets updates
- ✅ Persistent WhatsApp Web login
- ✅ Comprehensive error handling and logging
- ✅ Test mode for safe development

## 🚀 Quick Start

### Option 1: Web Form (Recommended for beginners)

1. **Set up Google Sheet:**
   - Create a new Google Sheet named "Badminton Bookings"
   - Add headers: `Names`, `Dates`, `Booking Status`

2. **Deploy Google Apps Script:**
   - Copy code from `Code.gs`
   - Deploy as web app with public access
   - Get the web app URL

3. **Update and host the form:**
   - Update `index.html` with your web app URL
   - Host on GitHub Pages, Netlify, or any static hosting service

4. **Share with your group:**
   - Share the form URL in your WhatsApp group
   - Members can book slots directly through the form

### Option 2: WhatsApp Bot (Advanced users)

1. **Set up Google Sheets API:**
   - Create Google Cloud project
   - Enable Google Sheets API
   - Create service account and download credentials
   - Share your Google Sheet with the service account

2. **Install and configure:**
   ```bash
   pip3 install -r requirements.txt
   # Update configuration in whatsapp_bot.py
   ```

3. **Run the bot:**
   ```bash
   python3 whatsapp_bot.py
   # Scan QR code on first run
   ```

## 📁 Project Structure

```
badminton-booking-system/
├── README.md                    # This file
├── index.html                   # Web form (complete, ready to use)
├── Code.gs                      # Google Apps Script code
├── whatsapp_bot.py             # Full WhatsApp bot implementation
├── test_bot.py                 # Test version for development
├── requirements.txt            # Python dependencies
├── deployment_instructions.md   # Detailed deployment guide
├── whatsapp_bot_setup.md       # WhatsApp bot setup instructions
├── web_form_plan.md            # Web form development plan
├── whatsapp_bot_plan.md        # WhatsApp bot development plan
└── todo.md                     # Project progress tracker
```

## 🎯 Use Cases

### Web Form Solution - Best For:
- ✅ Groups that prefer manual booking through a form
- ✅ Users who want a simple, reliable solution
- ✅ Situations where WhatsApp automation is not desired
- ✅ Quick setup with minimal technical requirements
- ✅ Free hosting and maintenance

### WhatsApp Bot Solution - Best For:
- ✅ Groups that want seamless WhatsApp integration
- ✅ Automatic booking without leaving the chat
- ✅ Advanced users comfortable with Python and APIs
- ✅ Groups that frequently use holiday/skip commands
- ✅ Scenarios requiring real-time automation

## ⚠️ Important Considerations

### Web Form Solution
- ✅ **Fully compliant** with all terms of service
- ✅ **No risk** of account bans or restrictions
- ✅ **Reliable** and stable long-term solution
- ✅ **Easy maintenance** and updates

### WhatsApp Bot Solution
- ⚠️ **Against WhatsApp's Terms of Service** - use at your own risk
- ⚠️ **Risk of phone number ban** - use secondary number recommended
- ⚠️ **Requires technical setup** - Google Cloud, Python, Chrome
- ⚠️ **May break** with WhatsApp Web updates

## 🛠️ Technical Requirements

### Web Form Solution
- Google account (for Google Sheets and Apps Script)
- Static web hosting (GitHub Pages, Netlify, etc.)
- Basic HTML/JavaScript knowledge for customization

### WhatsApp Bot Solution
- Python 3.7+
- Google Chrome browser
- Google Cloud account (for Sheets API)
- WhatsApp account (preferably secondary)
- Linux/Mac/Windows with Python support

## 📖 Documentation

- **[Deployment Instructions](deployment_instructions.md)** - Complete setup guide for both solutions
- **[WhatsApp Bot Setup](whatsapp_bot_setup.md)** - Detailed WhatsApp bot configuration
- **[Web Form Plan](web_form_plan.md)** - Web form development details
- **[WhatsApp Bot Plan](whatsapp_bot_plan.md)** - Bot development architecture

## 🧪 Testing

### Web Form Testing
The web form has been tested and includes:
- Form validation and error handling
- Google Apps Script integration
- Mobile responsiveness
- Cross-browser compatibility

### WhatsApp Bot Testing
Use the test version for safe development:
```bash
python3 test_bot.py
```

This tests Google Sheets integration and message parsing without WhatsApp Web.

## 🎨 Customization

### Web Form Customization
- **Styling:** Modify CSS in `index.html`
- **Fields:** Add/remove form fields as needed
- **Validation:** Update JavaScript validation rules
- **Branding:** Change colors, fonts, and layout

### Bot Customization
- **Message Patterns:** Update booking and holiday patterns
- **Check Interval:** Modify monitoring frequency
- **Date Format:** Change date formatting preferences
- **Commands:** Add new command types

## 🔒 Security & Privacy

### Web Form
- Uses HTTPS for secure data transmission
- Google Apps Script provides secure backend
- No sensitive data stored in frontend
- CORS protection built-in

### WhatsApp Bot
- Credentials stored locally in JSON file
- No message content stored permanently
- Google Sheets API uses OAuth2 authentication
- Chrome profile isolated for bot use

## 🆘 Troubleshooting

### Common Issues

**Web Form:**
- Form not submitting → Check Google Apps Script URL and permissions
- Data not in sheet → Verify script deployment and sheet sharing

**WhatsApp Bot:**
- Login issues → Clear browser profile and re-scan QR code
- Messages not detected → Check group name and message patterns
- Google Sheets errors → Verify service account permissions

See [Deployment Instructions](deployment_instructions.md) for detailed troubleshooting.

## 🤝 Contributing

This project is designed to be easily customizable for your specific needs:

1. **Fork the project** for your own group
2. **Customize the styling** and functionality
3. **Add new features** like member limits or payment tracking
4. **Share improvements** with the community

## 📄 License

This project is provided as-is for educational and personal use. 

**Important:** The WhatsApp bot component uses unofficial automation which violates WhatsApp's Terms of Service. Use responsibly and at your own risk.

## 🙏 Acknowledgments

- Google Apps Script for free backend hosting
- Selenium WebDriver for browser automation
- Google Sheets API for data storage
- Chrome WebDriver for WhatsApp Web automation

## 📞 Support

For setup help and troubleshooting:
1. Check the [Deployment Instructions](deployment_instructions.md)
2. Review the specific setup guides for your chosen solution
3. Test with the provided test versions
4. Verify all prerequisites are met

---

**Choose the solution that best fits your group's needs and technical comfort level. The web form solution is recommended for most users due to its simplicity and compliance with all terms of service.**


