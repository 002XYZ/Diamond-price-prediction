# Diamond-price-prediction
This work predicts the price class of a diamond based on the attributes given in the csv file.
The price attribute is numerical, but it is not practical doing regression analysis to predict the price.
When someone goes to buy jewellery, diamonds, in a shop, they don't state an exact price of the diamond they want to buy. Buyers will have a _price range_ within which they would be comfortable buying the diamond.
So, this problem is converted to a **classification problem**.
![image](https://github.com/002XYZ/Diamond-price-prediction/assets/75514397/4a29286b-ab2f-4999-9774-3e436a5ab647)

Classification is done in two ways:
* Binning price according to data points: As we can see from the boxplot that most of the diamonds are priced within the rough range of $800 to $5200. We create 10 bins, each of which will have equal number of data points. But it might happen that one bin can be, like say $1000 to $1010, and another bin can be $7000 to $8500.
* Binning price according to price: Now the more logical binning, we divide the diamonds into bins that are equally spaced. This will lead us to the scenario that some bins might have 1000 diamonds, and some bins only 2.

We also use two types of encoding, LabelEncoding and OneHotEncoding to convert the ordinal attributes into numerical ones.

We have used the classification models without modifying any hyperparametres, with both types of encoding and both types of binning.
We have done the same after tuning the hyperparametres too. We have some interesting findings in both the cases.
