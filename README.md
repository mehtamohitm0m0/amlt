# amlt

https://github.com/mehtamohitm0m0/amlt 
www.tiny.cc/amlt


Preprocessing ke codes 


# drop a single column by name
df = df.drop('B', axis=1)


# drop multiple columns by name
df = df.drop(['A', 'C'], axis=1)


# drop a single column by index
df = df.drop(df.columns, axis=1)


# drop multiple columns by index
df = df.drop(df.columns[[0, 2]], axis=1)




# create a sample DataFrame
df = pd.DataFrame({'color': ['red', 'green', 'blue', 'red', 'green']})


# perform one hot encoding of the 'color' column
df_encoded = pd.get_dummies(df['color'])




# create a LabelEncoder object
from sklearn.preprocessing import LabelEncoder
le = LabelEncoder()


# fit and transform the 'color' column
df['color_encoded'] = le.fit_transform(df['color'])


plt.figure(figsize=(8,6));
plt.scatter(X_pca[:,0],X_pca[:,1],c=y);
plt.xlabel('First principal component');
plt.ylabel('Second Principal Component');




