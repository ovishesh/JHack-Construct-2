# Game-Dev-Construct-2

### 1. [Introduction and Overview](/Content/Introduction.pptx)

### 2. Construct 2 - Showcase (Brian)

### 3. [AzureU Activation](https://www.microsoftazurepass.com/howto)

### 4. Project Preperation and Construction (Jason)

### 5. [Azure Overview](https://portal.azure.com)

### 6. Implementing Globals Scoring and Leaderboards(Jason)

1. [Setting up project to convert json to an array] (http://jamesqquick.com/json-to-construct-2-array/)
2. [Creating a table in Azure and then making a GET request and displaying the results to the user] (http://jamesqquick.com/construct-2-high-scores-with-azure-mobile-apps/)

Inserting the user's score into our table

``` var api = {
    post: function (request, response, next) {
        request.azureMobile.tables('UserScores')
            .insert({ name: request.query.name, score: request.query.score})
            .then(results => response.json(results))
            .catch(next);
    }
};

module.exports = api; ```

### 7. Facebook Integration(Jason or Brian)

### 8. Publish Game to Azure Web Apps(Brian)