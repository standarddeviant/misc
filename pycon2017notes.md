# Dave Crist's Pycon 2017 Notes

* The `dis` module lets you look at a lower level of a python function, like assembly for the python interpreter

# Videos
These are some links from the many Pycon 2017 youtube videos that I found interesting and relevant to my work or interests.

## Misc.
* [It's Time to Learn Regex](https://www.youtube.com/watch?v=abrcJ9MpF60)
* [How and When to use Fuzzy Search](https://www.youtube.com/watch?v=kTS2b6pGElE)
  * Using a SQL database, provides neat overview of 
    * Soundex
	* Levenshtein
	* N/Tri-Gram
	* NLTK: WordNet
	* Word2Vec (now in tensorflow)
* [State of Python Visualization Tools](https://www.youtube.com/watch?v=FytuB8nFHPQ)

## Maintaining an App/Package
* [Nice, Simple "all inclusive" basics overview to create a server-side app](https://www.youtube.com/watch?v=OaT0EN-02iY)
  * covers flask, sqllite, and basic python tools
  * good for beginners
  * fast-paced

* [How to share your code as a python package](https://www.youtube.com/watch?v=qOH-h-EKKac)
  * reccommends cookiecutter for things like license, readme, contributing, test boilerplate, etc.
  * https://packaging.python.org/ is the authoritative info on packaging 
  
  

## Asynchronous Programming
* [Interesting overview of python's async vs. os's threads/processes](https://www.youtube.com/watch?v=iG6fr81xHKA)
* [How-To-Use for async/await](https://www.youtube.com/watch?v=2ZFFv-wZ8_g)

## Statistics
* [Probablistic Programming, PyMC3 for Monte Carlo Simulations](https://www.youtube.com/watch?v=5TyvJ6jXHYE)
  * Bayes is useful due to its simplicity
  * Probabilistic Programming in 3 steps
    1. Encode a probabilities model
      * Specify your "priors" distribution or thing that models uncertainty: normal, beta, lognormal, etc.
      * Specify likelihood function, i.e. "data generating mechanism" or "how we update our prior probability"
      	* Again, could be normal, binomial, poisson
    2. Infer Values
      * Requires integration of $y$ over all parameters, and for many (100s or 1,000s)  variables, we need numerical methods
      * Probabilistic Programming abstracts the numerical methods, consider it a "black box"
    3. Check your model
      * Simulate data from your model, and plot them against histograms of observed data
    * Not new, WinBUGS was used in the 90s, but written in Objective Pascal...
    * PyMC3 uses theano with gradients for tensors
    
    






