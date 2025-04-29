# eecs182-homework-1-solved
**TO GET THIS SOLUTION VISIT:** [EECS182 Homework 1 Solved](https://www.ankitcodinghub.com/product/eecs182-solved-10/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;116533&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;2&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (2 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;EECS182 Homework 1  Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (2 votes)    </div>
    </div>
1. Bias-Variance Tradeoff Review

(a) Show that we can decompose the expected mean squared error into three parts: bias, variance, and irreducible error σ2:

Error = Bias2 + Variance + σ2

Formally, suppose we have a randomly sampled training set D (drawn independently of our test data), and we select an estimator denoted θ = θˆ(D) (for example, via empirical risk minimization). The expected mean squared error for a test input x can be decomposed as below:

EY ∼p(y|x),D[(Y − fθˆ(D)(x))2] = Bias(fθˆ(D)(x))2 + Var(fθˆ(D)(x)) + σ2

Bias(fθˆ(D)(x)) = EY ∼p(Y |x),D[fθˆ(D)(x) − Y ]

Var(fθˆ(D)(x)) = ED h(fθˆ(D)(x) − E[fθˆ(D)(x)])2i

(b) Suppose our training dataset consists of where the only randomness is coming from the label vector Y = Xθ∗ + ε where θ∗ is the true underlying linear model and each noise variable εi is i.i.d. with zero mean and variance 1. We use ordinary least squares to estimate a θˆ from this data. Calculate the bias and covariance of the θˆ estimate and use that to compute the bias and variance of the prediction at particular test inputs x. Recall that the OLS solution is given by

θˆ= (X⊤X)−1X⊤Y,

where X ∈ Rn×d is our (nonrandom) data matrix, Y ∈ Rn is the (random) vector of training targets.

For simplicity, assume that X⊤X is diagonal.

2. Least Squares and the Min-norm problem from the Perspective of SVD

Consider the equation Xw = y, where X ∈ Rm×n is a non-square data matrix, w is a weight vector, and y is vector of labels corresponding to the datapoints in each row of X.

Let’s say that X = UΣV T is the (full) SVD of X. Here, U and V are orthonormal square matrices, and Σ is an m × n matrix with non-zero singular values (σi) on the “diagonal”.

For this problem, we define Σ† an n × m matrix with the reciprocals of the singular values ( ) along the

“diagonal”.

(a) First, consider the case where m &gt; n, i.e. our data matrix X has more rows than columns (tall matrix) and the system is overdetermined. How do we find the weights w that minimizes the error between Xw and y? In other words, we want to solve minw ∥Xw − y∥2.

(b) Plug in the SVD X = UΣV T and simplify. Be careful with dimensions!

(c) You’ll notice that the least-squares solution is in the form w∗ = Ay. What happens if we leftmultiply X by our matrix A? This is why the matrix A of the least-squares solution is called the left-inverse.

(d) Now, let’s consider the case where m &lt; n, i.e. the data matrix X has more columns than rows and the system is underdetermined. There exist infinitely many solutions for w, but we seek the minimumnorm solution, ie. we want to solve min∥w∥2s.t.Xw = y. What is the minimum norm solution?

(e) Plug in the SVD X = UΣV T and simplify. Be careful with dimensions!

(f) You’ll notice that the min-norm solution is in the form w∗ = By. What happens if we right-multiply X by our matrix B? This is why the matrix B of the min-norm solution is called the right-inverse.

3. The 5 Interpretations of Ridge Regression

(a) Perspective 1: Optimization Problem. Ridge regression can be understood as the unconstrained optimization problem

argmin , (1) w

where X ∈ Rn×d is a data matrix, and y ∈ Rn is the target vector of measurement values. What’s new compared to the simple OLS problem is the addition of the λ∥w∥2 term, which can be interpreted as a “penalty” on the weights being too big.

Use vector calculus to expand the objective and solve this optimization problem for w.

(b) Perspective 2: “Hack” of shifting the Singular Values. In the previous part, you should have found the optimal w is given by

w = (XT X + λI)−1XT y

(If you didn’t get this, you should check your work for the previous part).

Let X = UΣV T be the (full) SVD of the X. Recall that U and V are square orthonormal (normpreserving) matrices, and Σ is a n × d matrix with singular values σi along the “diagonal”. Plug this into the Ridge Regression solution and simplify. What happens when the singular values when σi &lt;&lt; λ? What about when σi &gt;&gt; λ?

(c) Perspective 3: Maximum A Posteriori (MAP) estimation. Ridge Regression can be viewed as finding the MAP estimate when we apply a prior on the (now viewed as random parameters) W. In particular, we can think of the prior for√ W as being N(0,I) and view the random Y as being generated using

Y = xT W + λN where the noise N√ is distributed iid (across training samples) as N(0,1). At the

vector level, we have Y = XW + λN. Note that the X matrix whose rows are the n different training points are not random.

Show that (1) is the MAP estimate for W given an observation Y = y.

(d) Perspective 4: Fake Data. Another way to interpret “ridge regression” is as the ordinary least squares for an augmented data set — i.e. adding a bunch of fake data points to our data. Consider the following augmented measurement vector yˆ and data matrix Xˆ:

yˆ Xˆ ,

where 0d is the zero vector in Rd and Id ∈ Rd×d is the identity matrix. Show that the classical OLS optimization problem argminw has the same minimizer as (1).

(e) Perspective 5: Fake Features. For this last interpretation, let’s instead construct an augmented design matrix in the following way: √

Xˇ = [X λIn] √

i.e. we stack X with λIn horizontally. Now our problem is underdetermined: the new dimension d + n is larger than the number of points n. Therefore, there are infinitely many values η ∈ Rd+n for which Xˇη = y. We are interested in the min-norm solution, ie. the solution to

argmin s.t. Xˆη = y. (2) η

Show that this is yet another form of ridge regression and that the first d coordinates of η∗ form the minimizer of (1).

(f) We know that the Moore-Penrose pseudo-inverse for an underdetermined system (wide matrix) is given by A† = AT (AAT )−1, which corresponds to the min-norm solution for Aη = z. That is, the optimization problem

argmin∥η∥2s.t.Aη = z

is solved by η = A†z. Let wˆ be the minimizer of (1).

Use the pseudo-inverse to show that solving to the optimization problem in (2) yields

wˆ = XT (XXT + λI)−1y

Then, show that this is equivalent to the standard formula for Ridge Regression

wˆ = (XT X + λI)−1XT y

(g) We know that the solution to ridge regression (1) is given by wˆr = (X⊤X + λI)−1X⊤y. What happens when λ → ∞? It is for this reason that sometimes ridge regularization is referred to as “shrinkage.”

(h) What happens to the solution of ridge regression when you take the limit λ → 0? Consider both the cases when X is wide (underdetermined system) and X is tall (overdetermined system).

4. General Case Tikhonov Regularization

Consider the optimization problem:

x

Where W1, A, and W2 are matrices and x, b and c are vectors. W1 can be viewed as a generic weighting of the residuals and W2 along with c can be viewed as a generic weighting of the parameters.

(a) Solve this optimization problem manually by expanding it out as matrix-vector products, setting the gradient to 0, and solving for x.

(b) Construct an appropriate matrix C and vector d that allows you to rewrite this problem as

min∥Cx − d∥2 x

and use the OLS solution (x∗ = (CT C)−1CT d) to solve. Confirm your answer is in agreement with the previous part.

(c) Choose a W1, W2, and c such that this reduces to the simple case of ridge regression that you’ve seen in the previous problem, x∗ = (AT A + λI)−1AT b.

5. Coding Fully Connected Networks

In this coding assignment, you will be building a fully-connected neural network from scratch using NumPy. You will have the choice between two options:

Use Google Colab (Recommended). Open this url and follow the instructions in the notebook.

Use a local Conda environment. Clone https://github.com/gonglinyuan/cs182hw1 and refer to README.md for further instructions.

For this question, please submit a .zip file your completed work to the Gradescope assignment titled “Homework 1 (Code)”. Please answer the following question in your submission of the written assignment:

(a) Did you notice anything about the comparative difficulty of training the three-layer net vs training the five layer net?

6. Visualizing features from local linearization of neural nets

This problem expects you to modify the Jupyter Notebook you were given in the first discussion section for the course to allow the visualization of the effective “features” that correspond to the local linearization of the network in the neighborhood of the parameters.

We provide you with some starter code on Google Colab. For this question, please do not submit your code to Gradescope. Instead, just include your plots and comments regarding the questions in the subparts.

(a) Visualize the features corresponding to and where are the first hidden

layer’s weights and the are the first hidden layer’s biases. These derivatives should be evaluated at at least both the random initialization and the final trained network. When visualizing these features, plot them as a function of the scalar input x, the same way that the notebook plots the constituent “elbow” features that are the outputs of the penultimate layer.

(b) During training, we can imagine that we have a generalized linear model with a feature matrix corresponding to the linearized features corresponding to each learnable parameter. We know from our analysis of gradient descent, that the singular values and singular vectors corresponding to this feature matrix are important.

Use the SVD of this feature matrix to plot both the singular values and visualize the “principle features” that correspond to the d-dimensional singular vectors multiplied by all the features corresponding to the parameters.

(HINT: Remember that the feature matrix whose SVD you are taking has n rows where each row corresponds to one training point and d columns where each column corresponds to each of the learnable features. Meanwhile, you are going to be plotting/visualizing the “principle features” as functions of x even at places where you don’t have training points.)

(c) Augment the jupyter notebook to add a second hidden layer of the same size as the first hidden layer, fully connected to the first hidden layer. Allow the visualization of the features corresponding to the parameters in both hidden layers, as well as the “principle features” and the singular values.

7. Homework Process and Study Group

We also want to understand what resources you find helpful and how much time homework is taking, so we can change things in the future if possible.

(a) What sources (if any) did you use as you worked through the homework?

(b) If you worked with someone on this homework, who did you work with?

List names and student ID’s. (In case of homework party, you can also just describe the group.)

(c) Roughly how many total hours did you work on this homework? Write it down here where you’ll need to remember it for the self-grade form.

Contributors:

• Brandon Trabucco.

• Saagar Sanghavi.

• Alexander Tsigler.

• Anant Sahai.

• Jane Yu.

• Philipp Moritz.

• Soroush Nasiriany.

• Linyuan Gong.

• Sheng Shen.
