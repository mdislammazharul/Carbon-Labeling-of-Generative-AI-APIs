Here's a `README.md` file for your GitHub repository:

---

# Carbon-Labeling of Generative-AI APIs: User Behavior Study

## Overview

This project aims to investigate how **carbon labels on generative AI APIs** influence user behavior. Specifically, the research focuses on whether mandatory carbon labels—such as grams of CO₂ or equivalent car kilometers—can shift user choices when interacting with generative AI models. The study also explores which label format is most effective at driving conscious usage.

The goal is to push AI developers to incorporate **carbon emission rates** in their interfaces to promote responsible and sustainable use of AI technology.

## Research Question

**How much could mandatory carbon labels on generative-AI APIs shift user behavior, and what label format is most effective?**

## Why This Research is Novel

While carbon transparency in technology is often discussed, **no empirical study has yet tested actual user choices** regarding carbon labels on generative AI APIs. This research will help fill that gap and provide valuable insights into user behavior.

## Project Pipeline

1. **Front-End:** A simple HTML + JavaScript web interface for a mock API playground displaying three different carbon label formats:

   - Grams CO₂
   - Equivalent car kilometers
   - No label (control condition)

2. **Data Collection:** Participants (recruited from Prolific / social media) are asked to perform a 5-minute creative task. We track their interaction with the API and log the number of API calls they make, as well as the label format they were exposed to.

3. **Data Analysis:** The number of API calls across different label conditions is analyzed using a **t-test** to determine if carbon labeling has a significant effect on user behavior.

4. **Backend:** A lightweight backend captures participant data and logs interactions. The data is stored in a secure JSON format and will be deleted after the project concludes.

---

## How to Run

### Prerequisites

No special prerequisites are needed to run this project locally. You only need a basic web server to serve the `HTML, CSS, and JS` files.

### 1. Clone the repository

```bash
git clone https://github.com/mdislammazharul/Carbon-Labeling-of-Generative-AI-APIs.git
```

### 4. Open the webpage

Just click the `html` file to open it in a browser and go to. You should be able to interact with the mock API playground and participate in the study.

---

## Data Format

Participant data is recorded in the following format:

```json
{
  "record": {
    "action": "submit",
    "participantId": "2c89126f-fbf3-4340-bd3d-bc63e8326ff7",
    "consent": true,
    "startedAt": "2025-08-13T20:33:20.100Z",
    "endedAt": "2025-08-13T20:33:36.205Z",
    "timeSpentSec": 11,
    "demographics": {
      "age": "25-34",
      "gender": "Male",
      "country": "Bangladesh",
      "education": "Master’s",
      "employment": "Student",
      "techExp": "Advanced",
      "aiUse": "Daily",
      "envConcern": "Very concerned"
    },
    "apiCount": 1,
    "carbonGrams": 5,
    "apiCalls": [
      {
        "t": "2025-08-13T20:33:27.965Z",
        "promptLen": 13,
        "outputLen": 1036
      }
    ],
    "exitOpinionCarbonMeter": true
  },
  "metadata": {
    "id": "689cf6a0d0ea881f4058a0b0",
    "private": true,
    "createdAt": "2025-08-13T20:33:36.965Z"
  }
}
```

This JSON object contains:

- **User Consent**: Whether the participant has agreed to participate in the study.
- **Demographics**: Information about the participant (age, gender, country, etc.) that is logged for analysis purposes.
- **API Usage**: The number of API calls made during the task, as well as the corresponding carbon emission data (in grams CO₂).
- **Exit Opinion**: Whether the participant provided feedback on the carbon meter after completing the task.

---

## Contributing

Feel free to fork this project and contribute improvements or feature enhancements! You can also open an issue if you have any questions or suggestions for the project.

### Issues

- If you encounter any bugs or have suggestions for new features, please create an issue [here](https://github.com/mdislammazharul/Carbon-Labeling-of-Generative-AI-APIs/issues).

---

## Ethical Considerations

- **Voluntary Participation**: Participation in this study is entirely voluntary. Participants can withdraw at any time without penalty.
- **Anonymity**: No personal identifying information (such as names or IP addresses) will be collected. All data is logged anonymously.
- **Data Privacy**: The collected data will be stored in a secure JSON file and deleted after the completion of the research.

---

## License

Not available right now.

---

Let me know if you need any additional details or changes!
