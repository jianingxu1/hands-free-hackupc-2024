# Hands-Free: Alexa Skill for Warehouse Management

**Hands-Free** is an Alexa Skill designed to assist warehouse workers by enabling hands-free management of essential tasks such as creating order lists and locating products. Through voice commands, users can interact seamlessly with the system, allowing for greater convenience and efficiency in warehouse operations.

> **🏆 HackUPC 2024 Winner**: We were thrilled to win the Seidor Challenge at **HackUPC 2024** with this project. Our solution was recognized for its innovative approach to optimizing warehouse operations through voice-driven AI, which minimizes the need for physical input.

## Features

- **Voice-Activated Task Management**: Warehouse workers can use voice commands to create and manage order lists.
- **Product Lookup by Voice**: Users can locate products in the warehouse using simple voice commands.
- **Optimal Path Calculation**: The system calculates the most efficient route to pick products based on warehouse data.
- **Hands-Free Operation**: No need to physically interact with devices, improving worker efficiency.

## Project Overview

The main source code is located in the `lambda_function.py` file, which contains the core logic for the Alexa Skill, including the interaction between the user and the Alexa interface. Other key components of the project are organized into the following directories:

### How We Built It

- **Alexa Skills**: We implemented the conversational AI interface using Alexa Skills.
- **Product Name Matching**: Leveraged Levenshtein distance to match product names from a dataset, enabling accurate product identification.
- **AWS S3**: We stored product data on Amazon S3, ensuring reliable and scalable access to information.
- **Algorithms**: 
  - A **Dynamic Programming algorithm with bit masks** was used for smaller product lists to find the optimal path.
  - For larger product lists, we used **Simulated Annealing**, which provides near-optimal solutions with much faster computation times.
- **Python Scripts**: Several custom Python scripts were developed to format and generate product data for testing.

### Challenges We Faced

1. **Alexa Developer Skills Console**: Debugging was challenging due to limited error reporting and low transparency.
2. **Product Name Parsing**: Common models struggled with parsing unconventional product names, which led us to implement a custom solution using Levenshtein distance.

## Contributors

- [Team Member](https://github.com/jianingxu1)
- [Team Member](https://github.com/jordimunozflorensa)
- [Team Member](https://github.com/yiqizhengshan)
- [Team Member](https://github.com/Farrius)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
