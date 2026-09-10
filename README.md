[README_16.md](https://github.com/user-attachments/files/32061102/README_16.md)
```python
movies = ["Jawan", "Pathaan", "Animal", "Stree ", "Pushpa 2"]

movie = iter(movies)

print(next(movie))
print(next(movie))
print(next(movie))
print(next(movie))
print(next(movie))
```

```python
songs = ["Kesariya", "Tum Hi Ho", "Apna Bana Le", "Heeriye", "Perfect", "Believer"]

for i, song in enumerate(songs, 1):
    print(i, ".", song)
```

```python
food = ["Pizza", "Burger", "Pasta", "Sandwich", "Biryani"]
prices = [250, 150, 200, 120, 300]

for item, price in zip(food, prices):
    print(item, "-", "₹" + str(price))
```

```python
def insta_posts_generator(posts):
    for post in posts:
        yield post
posts = ["Good vibes!", "Weekend mood", "New day!", "Keep going!"]

post = insta_posts_generator(posts)

while True:
    try:
        print(next(post))
    except StopIteration:
        break
```

```python
def cashback_generator(transactions):
    for amount in transactions:
        yield amount * 0.05

transactions = [100, 500, 1000, 200, 800]

for cashback in cashback_generator(transactions):
    print(cashback)
```
