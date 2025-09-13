# Ballerina Commons

**🚀 Comprehensive Utility Modules for Modern Ballerina Development**

Welcome to **Ballerina Commons** - a curated collection of powerful, production-ready utility modules designed to enhance your Ballerina development experience. Our mission is to provide the essential building blocks that every modern application needs, from time manipulation to string processing and beyond.

---
## 🌟 Vision

**Empowering Ballerina developers with comprehensive, intuitive, and powerful utility modules that make complex operations simple and reliable.**

We believe that developers should focus on building amazing applications, not reimplementing common functionality. Ballerina Commons bridges the gap between the standard library and real-world application needs, providing battle-tested utilities that handle the complexities so you don't have to.

## 🎯 Why Ballerina Commons?

### 🔧 **Production-Ready Utilities**
Every module is built with production use in mind - comprehensive error handling, extensive testing, and performance optimization.

### 🎨 **Developer Experience First**
Intuitive APIs, comprehensive documentation, and consistent patterns across all modules make development faster and more enjoyable.

### 🌍 **Modern Integration**
Built for today's applications with cross-platform compatibility, AI/ML readiness, and cloud-native features.

### ⚡ **Performance Focused**
Efficient implementations built on solid foundations with minimal overhead and maximum throughput.

## 📦 Available Modules

### 🕒 [TimePlus](https://github.com/ballerina-commons/module-commons-timeplus) - Comprehensive Time Utilities

*Making time simple, powerful, and intuitive in Ballerina! ⏰✨*

**TimePlus** extends the standard `ballerina/time` module with real-world functionality for modern applications:

- **🌍 Cross-Platform Integration**: Native support for JavaScript, Python, and Unix timestamps
- **🏢 Business Logic**: Weekend/weekday detection, business day calculations  
- **📅 Comprehensive Operations**: Time arithmetic, component extraction, range validation


### 🔤 [Strings](https://github.com/ballerina-commons/module-commons-strings) - Comprehensive String Utilities

*Making string manipulation simple, powerful, and intuitive in Ballerina! 🔤✨*

**Strings** provides powerful, real-world functionality for string manipulation, cleaning, formatting, and processing:

- **🔄 Case Transformations**: camelCase, snake_case, kebab-case, Title Case conversions
- **🧼 Cleaning & Sanitization**: Text cleaning, whitespace handling, character filtering
- **📏 Padding & Truncation**: Smart padding and truncation with multiple strategies
- **🛡️ Safe Operations**: Null-safe operations with sensible defaults
- **🤖 AI/LLM Ready**: Masking, redaction, and token-aware truncation


## 🚀 Getting Started

### Installation

Add any module to your Ballerina project by adding import statements.

```ballerina
// main.bal

import commons/timeplus;
import commons/strings;

```

### Quick Usage

```ballerina
import commons/timeplus;
import commons/strings;

public function main() returns error? {
    // Time operations
    time:Utc now = timeplus:now();
    string timestamp = check timeplus:toString(now, timeplus:ISO_8601);
    
    // String operations  
    string processedName = strings:toTitleCase(strings:trimAndClean(userInput));
    string maskedCard = strings:maskCreditCard(creditCardNumber);
}
```

## 🤝 Contributing

We welcome contributions from the Ballerina community! Here's how you can help:

### **Ways to Contribute**
- 🐛 **Report Issues**: Found a bug? Let us know!
- 💡 **Suggest Features**: Have an idea? We'd love to hear it!
- 📖 **Improve Documentation**: Help make our docs even better
- 🔧 **Submit Code**: Fix bugs or implement new features
- 🧪 **Add Tests**: Help us maintain our high testing standards

### **Development Setup**
```bash
# Clone any module repository
git clone https://github.com/ballerina-commons/module-commons-timeplus.git
cd module-commons-timeplus

# Build and test
bal build
bal test
```

### **Contribution Guidelines**
- Follow existing code style and patterns
- Add comprehensive tests for new functionality
- Update documentation for any API changes
- Ensure all tests pass before submitting

## 📋 Roadmap

### **Upcoming Modules**
- **🔢 Numbers**: Advanced numeric operations, formatting, and calculations
- **📊 Collections**: Enhanced array, map, and set utilities
- **🌐 Network**: HTTP utilities, URL manipulation, and network helpers
- **📄 Files**: File system operations and data processing

### **Module Enhancements**
- **TimePlus**: Enhanced timezone support, calendar systems
- **Strings**: Additional format support, advanced text processing


## 📄 License

All modules in Ballerina Commons are licensed under the **Apache License 2.0**.

## 📞 Support & Community

- **📖 Documentation**: Comprehensive docs in each module repository
- **🐛 Issues**: Report bugs and request features via GitHub Issues
- **💬 Discussions**: Join our community discussions on GitHub
- **📧 Contact**: Reach out to maintainers for questions or collaboration

## 🏆 Attribution

**Ballerina Commons** is created and maintained by **[Hasitha Aravinda](https://github.com/hasithaa)**.

### About the Author

**Hasitha Aravinda** brings extensive expertise to Ballerina Commons as the former **Lead Developer of the Ballerina Compiler Team** and one of the **primary contributors to the Ballerina Language Design**. With **12+ years of experience in integration spaces** working directly with customers, this project represents an attempt to distill that real-world experience into reusable, production-ready utility modules.

This deep understanding of both the Ballerina language internals and practical integration challenges ensures that every module in Ballerina Commons addresses genuine developer pain points with well-designed, efficient solutions.

### Community

Special thanks to all contributors who help make these utilities better for everyone in the Ballerina ecosystem.

## 🔗 Related Projects

- **[Ballerina Language](https://github.com/ballerina-platform/ballerina-lang)** - The Ballerina programming language
- **[Ballerina Central](https://central.ballerina.io/)** - Ballerina package repository

---

**💡 Have an idea for a new utility module?** Open an issue and let's discuss how we can make Ballerina development even better!

**🌟 Star our repositories** if you find these utilities helpful!

---

## Notice:

*Ballerina is a registered trademark of WSO2 LLC.*