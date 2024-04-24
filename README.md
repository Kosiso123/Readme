# FRONTEND LOW LEVEL DESIGN DOCUMENT
## Insight Feature

### Insight Feature: This is the overall feature within the farmer app that provides insights about GMO crops and farming practices.
**Component Tree**

- Insight Feature
  - Main Page
    - Insight List
      - Insight Card 1
      - Insight Card 2
      - Insight Card 3
      ...
  - Individual Insight Page
    - Insight Details
      - Title
      - Description
      - Author
      - Date
      - Content
- Filter
- Search Bar
- Insight Feature: This is the overall feature within the farmer app that provides insights about GMO crops and farming practices.
- Main Page: This is the first page users see when they access the Insight feature. It typically includes a list of insights displayed as cards or tiles. Users can scroll through this list to see all available insights.
- Insight List: This is a component within the main page that contains all the insights available to users. It organizes and presents the insights in a visually appealing way, such as a grid or a list.
- Insight Card: Each insight in the list is represented by an insight card. These cards provide a brief overview of the insight, including its title, author, and a short description. Users can click on a card to view the full details of the insight.
- Individual Insight Page: When a user clicks on an insight card, they are taken to the individual insight page, which displays the full details of that specific insight.
- Insight Details: This component contains all the details of the insight, such as its title, description, author, date of publication, and the content itself. Users can read through this information to learn more about the insight and its relevance to GMO crops and farming practices.

  ![Screenshot_20240424-213639](https://github.com/Kosiso123/Readme/assets/150237235/40872fb2-bc73-4da9-932d-d3dbd7501c1d)


  **Filter and Search Bar Components**

**Introduction:**
The filter and search bar components are essential features of the Insight page in the farmer app, allowing users to narrow down and search for specific insights based on their preferences and interests.

**Implementation Steps:**

1. **Filter Component:**
   - Design a user interface to present filter options to the user.
   - Attach event listeners to filter inputs to detect changes.
   - Implement JavaScript functions to dynamically filter insights based on selected criteria.
   - Update the UI to reflect filtered insights.

2. **Search Bar Component:**
   - Design a search bar UI element with a text input field and a search button/icon.
   - Capture user input and trigger search queries on input change or submission.
   - Implement search logic to filter insights based on entered keywords.
   - Display search results to the user, highlighting matching keywords or phrases.


**Example Code Snippets:**

**Filter Component:**
    ```javascript
    // Function to filter insights based on selected criteria
    function filterInsights(criteria) {
    // Filter insights based on criteria
    // Update UI to reflect filtered insights
    }

    // Function to search insights based on entered keywords
    function searchInsights(query) {
    // Search through insights for matching keywords
    // Display search results to the user
    }





    

## How Each Component Interact With Each Other

To address the requirement of well-defined state shapes and component contracts for the Insight feature, we need to outline the specific information each component will require and how they will interact with each other. Here's how we can define this for the Insight feature:

- **Insight Card Component:**
- **Requires:** Title, Description, Author
- **Interaction:** Displays information about each insight in a concise fo  rmat.
- **Insight List Component:**
- **Requires:** List of Insights
- **Interaction:** Receives a list of insights and renders them using Insight Card components.
