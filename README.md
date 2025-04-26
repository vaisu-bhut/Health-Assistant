# AI-Powered Personalized Health Assistant

## Project Overview
The AI-Powered Personalized Health Assistant leverages advanced Generative AI techniques to provide users with personalized fitness and nutrition recommendations. Utilizing fine-tuned large language models and structured workflow management, the assistant offers individualized health guidance tailored to diverse user profiles and goals.

---

## Team
- Kanika Rawat
- Vasu Vinodbhai Bhut
- Krupali Gunvantbhai Tejani

---

## Technologies Used
- **OpenAI API**: Access and fine-tuning of language models
- **Pandas, NumPy**: Data manipulation
- **Scikit-learn**: Machine learning utilities
- **LangChain, LangGraph**: Workflow management
- **Streamlit**: User interface development

---

## Features

### Personalized Recommendations
- Tailored workout routines
- Customized dietary guidelines
- Continuous engagement and motivation through interactive messaging

### Structured Workflow
- **Node Functions**:
  - `generate_workout_plan`
  - `generate_diet_plan`
  - `format_response`
- Directed Graph-based workflow ensuring coherent response integration
- State management via TypedDict for workflow consistency

### Prompt Engineering & Fine-Tuning
- Techniques Explored:
  - Zero-Shot Prompting
  - Few-Shot Prompting
  - Chain-of-Thought (CoT) Prompting
- Fine-tuning executed on **GPT-3.5-Turbo** with custom dataset, enhancing health domain relevance

### Robust Security Implementation
- **PromptDefender Class**:
  - Regular expression-based pattern matching
  - Context-sensitive validation
  - Prevention against encoding-based attacks
- **Multi-Stage Security Pipeline**:
  - Input sanitization
  - Secure query processing
  - Output validation

### User Interface with Streamlit
- User Profile Management
  - Physical attributes, dietary preferences, health goals
- Interactive Chat Interface
  - Conversation tracking and response rating
- Admin Dashboard
  - Metrics monitoring including response times, user ratings, and query volumes

---

## Security and Ethical Considerations
- Anonymous interactions (no personal data stored)
- Stateless and session-based responses
- Explicit disclaimer against providing medical diagnoses
- No medication or clinical treatment advice
- Ethical dataset usage (public and anonymized data)

---

## Challenges and Solutions

### Challenge: Fine-Tuning Data Quality
- **Problem**: Initial fine-tuning was inconsistent due to limited quality and diversity of data.
- **Solution**: Enhanced data generation with broader demographics, expert-reviewed responses, and rigorous data validation.

### Challenge: Prompt Injection Vulnerabilities
- **Problem**: System initially susceptible to prompt injection attacks.
- **Solution**: Developed the comprehensive PromptDefender class incorporating context-aware validation and thorough input/output sanitization.

### Challenge: Response Coherence
- **Problem**: Disjointed workout and nutrition advice.
- **Solution**: Implemented structured LangGraph workflow to integrate domain-specific advice effectively.

### Challenge: Performance Optimization
- **Problem**: Slow response times with complex queries.
- **Solution**: Introduced caching, optimized prompts, asynchronous processing, and fallback models.

---

## Performance Metrics
- **Response Quality**: Enhanced significantly post fine-tuning
- **Security Efficacy**: Successfully blocked 91% of prompt injection attempts
- **Average Response Time**: Reduced to 17.90 seconds for complex queries
- **User Satisfaction**: Positive feedback for personalized recommendations

---

## Future Vision
- Integration with wearable devices for real-time health data
- Expansion into mental health and chronic disease management
- Clinical validation to enhance reliability and impact

---

## References
- Artificial Intelligence in public health nutrition, personalized AI nutritionist
- Google's Personal Health Large Language Model (PH-LLM)
- ACE Fitness insights on AI in health and fitness
- MDPI review on AI and personalized nutrition
- Evaluation of AI virtual health assistants

---

## Project Repository
For complete source code and further details, visit the project repository (https://github.com/vaisu-bhut/Health-Assistant.git).

---

**Project Developed for:**  
Prompt Engineering for Generative AI  
Professor: Shirali Patel  