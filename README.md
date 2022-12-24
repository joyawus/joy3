# FINAL-PROJECT3

# Editting the file

It's a markdown file in this repository./
# Write your code here
df=pd.read_csv("exchange_rates.csv")

df.rename( columns={'Unnamed: 0':'Pounds'}, inplace=True )
df1=df.loc[df["Pounds"] == 'GBP']
df1
exchange_rate=float(df1["Rates"].values)
print(exchange_rate)
