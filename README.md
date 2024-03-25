# SUMMARY
The GroupLens Research Project is a research group in the Department of Computer Science and Engineering in the University of Minnesota. The researchers of this group are involved in many research projects related to the fields of information filtering, collaborative filtering, and recommender systems. Here, we ask you to perform the analysis using the Exploratory Data Analysis technique. In particular, we want you to apply the tools of machine learning to predict the survivors of the tragedy. 

# RATINGS FILE DESCRIPTION

All ratings are contained in the file "ratings.dat" and are in the
following format:

UserID::MovieID::Rating::Timestamp

- UserIDs range between 1 and 6040 
- MovieIDs range between 1 and 3952
- Ratings are made on a 5-star scale (whole-star ratings only)
- Timestamp is represented in seconds since the epoch as returned by time(2)
- Each user has at least 20 ratings

# USERS FILE DESCRIPTION

User information is in the file "users.dat" and is in the following
format:

UserID::Gender::Age::Occupation::Zip-code

All demographic information is provided voluntarily by the users and is
not checked for accuracy.  Only users who have provided some demographic
information are included in this data set.

- Gender is denoted by a "M" for male and "F" for female
- Age is chosen from the following ranges:

	*  1:  "Under 18"
	* 18:  "18-24"
	* 25:  "25-34"
	* 35:  "35-44"
	* 45:  "45-49"
	* 50:  "50-55"
	* 56:  "56+"

- Occupation is chosen from the following choices:

	*  0:  "other" or not specified
	*  1:  "academic/educator"
	*  2:  "artist"
	*  3:  "clerical/admin"
	*  4:  "college/grad student"
	*  5:  "customer service"
	*  6:  "doctor/health care"
	*  7:  "executive/managerial"
	*  8:  "farmer"
	*  9:  "homemaker"
	* 10:  "K-12 student"
	* 11:  "lawyer"
	* 12:  "programmer"
	* 13:  "retired"
	* 14:  "sales/marketing"
	* 15:  "scientist"
	* 16:  "self-employed"
	* 17:  "technician/engineer"
	* 18:  "tradesman/craftsman"
	* 19:  "unemployed"
	* 20:  "writer"

# MOVIES FILE DESCRIPTION

Movie information is in the file "movies.dat" and is in the following
format:

MovieID::Title::Genres

- Titles are identical to titles provided by the IMDB (including
year of release)
- Genres are pipe-separated and are selected from the following genres:

	* Action
	* Adventure
	* Animation
	* Children's
	* Comedy
	* Crime
	* Documentary
	* Drama
	* Fantasy
	* Film-Noir
	* Horror
	* Musical
	* Mystery
	* Romance
	* Sci-Fi
	* Thriller
	* War
	* Western

- Some MovieIDs do not correspond to a movie due to accidental duplicate
entries and/or test entries
- Movies are mostly entered by hand, so errors and inconsistencies may exist


# TASKS TO BE PERFORMED
### Data Acquisition
- Data acquisition of the MovieLens dataset, including:
  - Users dataset
  - Rating dataset
  - Movies dataset

### Exploratory Data Analysis (EDA) for Users Dataset
- Visualize user age distribution
- Visualize overall rating by users
- Visualize overall rating by gender
- Find and visualize the user rating of the movie “Toy Story”
- Find and visualize the viewership of the movie “Toy Story” by age group
- Find and visualize the top 25 movies by viewership rating
- Find the rating for a particular user with user id = 2696
  - Visualize the rating data for user id = 2696

### Machine Learning on First 500 Extracted Records
- Perform machine learning on the first 500 extracted records
- Use the following features:
  - Movie ID
  - Age
  - Occupation
- Use rating as the label

### Train and Test Data Preparation
- Create train and test datasets and perform the following:
  - Create a histogram for movie, age, and occupation

# RESULTS
<table>
  <tr>
    <td>Distribution of users by Age Group</td>
  </tr>
  <tr>
    <td><img src="https://github.com/Prince-hash-lab/Movie-lens-case-study-/blob/main/images/1.png" width=500 height=420></td>
  </tr>
 </table>

<table>
  <tr>
    <td>Overall Rating Count By Users</td>
  </tr>
  <tr>
    <td><img src="https://github.com/Prince-hash-lab/Movie-lens-case-study-/blob/main/images/2.png" width=700 height=610></td>
  </tr>
 </table>

 <table>
  <tr>
    <td>Distribution of users by Gender</td>
  </tr>
  <tr>
    <td><img src="https://github.com/Prince-hash-lab/Movie-lens-case-study-/blob/main/images/3.png" width=500 height=450></td>
  </tr>
 </table>

 <table>
  <tr>
    <td>User Rating of Movie Toy Story</td>
  </tr>
  <tr>
    <td><img src="https://github.com/Prince-hash-lab/Movie-lens-case-study-/blob/main/images/8.png" width=650 height=650></td>
  </tr>
 </table>

 <table>
  <tr>
    <td>Viewership Data of Toy Story Movie by Age</td>
  </tr>
  <tr>
    <td><img src="https://github.com/Prince-hash-lab/Movie-lens-case-study-/blob/main/images/5.png" width=750 height=480></td>
  </tr>
 </table>

 <table>
  <tr>
    <td>Top 25 Movies by Average Rating</td>
  </tr>
  <tr>
    <td><img src="https://github.com/Prince-hash-lab/Movie-lens-case-study-/blob/main/images/6.png" width=650 height=450></td>
  </tr>
 </table>

 <table>
  <tr>
    <td>Rating Data for User 2696</td>
  </tr>
  <tr>
    <td><img src="https://github.com/Prince-hash-lab/Movie-lens-case-study-/blob/main/images/7.png" width=500 height=450></td>
  </tr>
 </table>
