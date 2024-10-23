**BRIEFING THE PROJECT**

**1. Model Selection**
  -> The primary model used for this project is Mistral 7B, which was accessed via the Hugging Face Hub. Mistral 7B is a large-scale transformer-based language model suitable for tasks involving natural language generation, including text generation and classification tasks like genre prediction.
  
  -> **Chosen Models:** Mistral 7B was selected due to its ability to generate coherent and creative outputs. Additionally, models like LLaMA 3, GPT-2, and Google PaLM were also considered, but due to resource limitations in Colab, Mistral 7B was the preferred choice.
  
  -> **Genre Prediction Accuracy:** The Mistral 7B model achieved nearly 80% accuracy for genre prediction tasks, a satisfactory performance given the dataset and the complexity of multi-label genre classification.

**2.  Implementation Details**
  -> **Platform:** The project was implemented using Google Colab, with access to the models provided through the Hugging Face Hub. Colab’s free tier was initially used, leading to several limitations in terms of RAM and GPU allocation.
  
  -> **Tasks Performed:**

    1. **Movie Descriptions:** The model was used to generate creative and detailed descriptions of movies.
    2. **Genre Prediction:** Mistral 7B was tasked with predicting movie genres based on a given set of attributes like plot, cast, and keywords.
    3. **Plot Twists and Endings:** The model generated alternate plot twists and movie endings, demonstrating its capability for creative storytelling.
    
  -> **Pipeline Optimization:** A significant amount of time was spent optimizing the input prompt templates for Mistral 7B to ensure more reliable and coherent outputs. These prompts made the outputs more presentable.

**3. Challenges Faced**
  (i) **Memory Limitations:** When initially attempting to load Mistral 7B in Google Colab, the system ran out of memory as the RAM exceeded the 12GB limit. This led to multiple crashes and forced experiments with different model sizes and configurations.
  (ii) **GPU Resource Constraints:** While using larger models like LLaMA 3 and Mistral 7B, the available GPU in Google Colab hit the usage limit twice. This required careful management of GPU resources and switching between models like GPT-2 and Google PaLM to avoid further resource exhaustion.
  (iii) **Template Experimentation:** A significant challenge was experimenting with various input templates to get Mistral 7B to produce reliable outputs. The initial templates led to inconsistent results, so several iterations of prompt engineering were necessary to improve the model's performance for generating descriptions and predicting genres.

**4. Evaluation of the Model**
  (i) **Genre Prediction Accuracy:** The model’s performance was evaluated based on its genre prediction capabilities, which achieved an accuracy of approximately 80%. This was a good outcome given the complexity of movie genres, where a single movie can belong to multiple categories.
  (ii) **Quality of Generated Text:** The text generated for movie descriptions and plot twists was evaluated qualitatively, focusing on coherence, creativity, and relevance to the movie data provided. The model successfully generated meaningful alternate endings and creative twists that aligned with the given plot, demonstrating its effectiveness for creative writing tasks.
  (iii) **Human Feedback:** Given the nature of the outputs (creative descriptions and twists), human feedback was essential for evaluating the quality. Subjective assessments were made to judge the originality and logical consistency of the model's responses.

