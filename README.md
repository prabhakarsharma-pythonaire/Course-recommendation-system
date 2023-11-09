# Course-recommendation-system
This Coursera course recommendation system utilizes TF-IDF and cosine similarity for personalized suggestions. Handling abbreviations, it filters courses by difficulty and rating, providing a curated list. Users get detailed info on the top match, fostering a tailored learning experience.


This project serves as an intelligent recommendation system designed to assist users in discovering relevant online courses from Coursera. Leveraging a comprehensive dataset encompassing crucial details about each course, such as the course name, university, difficulty level, course rating, and a detailed course description, this system employs advanced techniques to enhance the user experience.

To begin with, the dataset is loaded and processed using the powerful pandas and numpy libraries in Python. The course features are enriched through the creation of a combined feature, incorporating the course name, university, difficulty level, and course description. This amalgamated feature undergoes transformation into numerical data through the application of TF-IDF (Term Frequency-Inverse Document Frequency) vectorization, a natural language processing technique. Subsequently, the cosine similarity metric is harnessed to gauge the similarity between different courses based on their textual features.

The system demonstrates user-centricity by accommodating common abbreviations. For instance, if a user inputs "ml" or "m.l.," the system intelligently translates it into "Machine Learning." Similarly, "ai" or "a.i." is transformed into "Artificial Intelligence," enhancing the user-friendly nature of the interface.

Upon user input of a specific course name, the recommendation system utilizes the difflib library to find the closest matching courses within the dataset. The user is prompted to specify their desired difficulty level, ranging from Beginner to Advanced, and input a minimum course rating. The system then filters courses based on these criteria and sorts them by similarity, offering a curated list of suggestions.

The final output presents the user with the top matching course, considering their specified difficulty level, rating, and the highest similarity score. The user receives comprehensive information about the recommended course, including its name, difficulty level, and rating. Additionally, the system is poised to display the course URL, facilitating seamless navigation to the suggested course.

In essence, this recommendation system amalgamates data preprocessing, natural language processing, and user-friendly input handling to provide a tailored and insightful selection of online courses. It empowers users to explore and engage with courses that align with their preferences and learning objectives, fostering a personalized and enriching educational journey on the Coursera platform.
