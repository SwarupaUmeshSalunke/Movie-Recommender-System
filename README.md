**Movie Recommender System 🎥**
A simple Movie Recommender System built using Machine Learning that suggests movies based on user-selected preferences. This application uses the TMDB dataset for movie information and employs the TMDB API to fetch movie posters dynamically.

**Features**
Interactive Interface: Easy-to-use interface built with Streamlit.
Movie Recommendations: Suggests similar movies based on the selected movie.
Dynamic Poster Fetching: Fetches movie posters from TMDB API to enhance the recommendation experience.
Collaborative Filtering: Uses a pre-trained similarity model for recommending movies.
Tech Stack
Python: Core language used for building the application.
Streamlit: Used for creating the interactive web interface.
Pandas: For data manipulation and handling movie data.
Pickle: For loading pre-trained models and movie data.
Requests: To interact with the TMDB API and fetch movie posters.
Installation and Setup
Clone the Repository:

**bash**
Copy code
git clone https://github.com/your-username/Movie-Recommender-System.git
cd Movie-Recommender-System
Install the Required Libraries:

**bash**
Copy code
pip install -r requirements.txt
Ensure the following libraries are included in the requirements.txt file:

**Copy code**
streamlit
pandas
requests
pickle-mixin
Download Necessary Files:

Ensure you have the movie_dict.pkl and similarity.pkl files in the project directory. These files contain the movie data and the similarity model.
Run the Streamlit App:

**bash**
Copy code
streamlit run app.py
Replace app.py with the filename containing the code above.

**Usage**
Launch the app using the above command.
Use the dropdown to select a movie from the list.
Click on the "Recommend" button to get the top 5 recommended movies along with their posters.
How It Works
Fetching Movie Posters: The fetch_poster(movie_id) function uses the TMDB API to get movie posters based on the movie ID.

**Recommendation System**: The recommend(movie) function fetches the most similar movies to the one selected by the user using a pre-trained similarity model.

**Interactive UI**: The app displays the recommended movies and their posters using Streamlit's column layout for a visually appealing presentation.

**API Key Configuration**
Ensure your TMDB API key is correctly set in the fetch_poster() function. Replace the placeholder in the code if needed:

**python**
Copy code
'https://api.themoviedb.org/3/movie/{}?api_key=YOUR_API_KEY&language=en-US'

**Screenshots**

