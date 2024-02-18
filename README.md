# Collaborative-filtering-recommander
Collaborative filtering is a recommendation technique that relies on collecting and analyzing user interactions, behaviors, or preferences to make predictions and suggest items or content that users might find relevant. 

# Collaborative Filtering

Collaborative Filtering is a powerful recommendation technique explored in this repository through a Jupyter Notebook. This technique relies on the analysis of user interactions, behaviors, or preferences to make predictions and suggest items that users might find relevant. The notebook begins by introducing the concept, emphasizing the assumption that users who agreed in the past tend to agree in the future. Recommendations are made based on similarities between users or items, providing personalized suggestions in domains such as movies, music, or products.

## Key Points:
- The notebook explores both user-based and item-based collaborative filtering methods.
- In practice, the item-item approach often outperforms the user-user approach in many use cases.
- Items are considered 'simpler' than users due to their belonging to a small set of 'genres,' making item similarity more meaningful than user similarity.

## Data Processing:
- Data cleaning involves handling invalid entries and ensuring data integrity.
- Centering of ratings is performed to address variations in user rating tendencies.

## Sparse Matrix and Similarity Computation:
- The notebook creates a sparse matrix using the CSR format to efficiently represent user-item interactions.
- Cosine similarity is computed between users based on their centered ratings.

## Functions:
- `get_user_bestMovies(user_id)`: Returns a list of movies highly rated by a specific user.
- `get_simillar_user(user_id)`: Returns indices of users similar to a specified user.
