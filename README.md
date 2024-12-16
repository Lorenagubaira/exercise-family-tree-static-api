<!-- hide -->
# Family Tree Static API
<!-- endhide -->

Based on the technologies/strategies we've learn build a static API that handles a family tree. You're free to use your own family information, you can use fake data too.

<onlyfor saas="false" withBanner="false">

## 🌱  How to start this project

Do not clone this repository because we will use a different template.  

We recommend opening the `python boilerplate` or `nodejs boilerplate` using a provisioning tool like [Codespaces](https://4geeks.com/lesson/what-is-github-codespaces) (recommended) or [Gitpod](https://4geeks.com/lesson/how-to-use-gitpod). Alternatively, you can [clone the GitHub repository](https://4geeks.com/how-to/github-clone-repository) on your local computer using the `git clone` command.  

Here are the repositories you can open or clone:  

- Python:  
```sh  
$ git clone https://github.com/4GeeksAcademy/flask-rest-hello  
```  
- Nodejs:  
```sh  
$ git clone https://github.com/4GeeksAcademy/expressjs-rest-hello  
```  

💡 Important: Remember to create a new repository, update the remote (`git remote set-url origin <your new url>`), and upload the code to your new repository using `add`, `commit`, and `push`.  

</onlyfor>

## 📝 Instructions

Your API must have, at least, 7 members spread throughout 3 generations:

```txt
grandparent -> parent -> current generation
```

The family tree must be represented as an object tree structure, i.e.: each person (node in the tree) must have: id, name, last-name, age, and a reference (id) to its parents and children (if any).

- `GET /all` The API must expose an endpoint that returns the full list of family members ordered by oldest to younger.
- `GET /member/<int:id>` The API must expose an endpoint that returns a specific member of the family tree by their id (which should be unique) and the information about its children and parents.

### Technologies

The API must be developed using **Flask** or **Expressjs** and each endpoint must return a *valid* **JSON** file.

### 💡 Hints

You may want to draw (pen and paper) the tree structure to have a "visual" structure in mind. Use the lines to display the references between parents and children.

The references should be the members' id numbers.

Create your data structures before you create the endpoints, use global variables.
  
