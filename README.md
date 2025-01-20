# goit-algo2-hw-08

## SlidingWindowRateLimiter

File [sliding_window_rate_limiter.py](./sliding_window_rate_limiter.py) contains the implementation of the sliding window rate limiter class.
Can be checked by build-in test cases in the file

```sh
python sliding_window_rate_limiter.py
```

Output:

```log
=== Симуляція потоку повідомлень ===
Повідомлення  1 | Користувач 2 | ✓
Повідомлення  2 | Користувач 3 | ✓
Повідомлення  3 | Користувач 4 | ✓
Повідомлення  4 | Користувач 5 | ✓
Повідомлення  5 | Користувач 1 | ✓
Повідомлення  6 | Користувач 2 | × (очікування 7.7с)
Повідомлення  7 | Користувач 3 | × (очікування 7.4с)
Повідомлення  8 | Користувач 4 | × (очікування 7.7с)
Повідомлення  9 | Користувач 5 | × (очікування 7.0с)
Повідомлення 10 | Користувач 1 | × (очікування 7.4с)

Очікуємо 4 секунди...

=== Нова серія повідомлень після очікування ===
Повідомлення 11 | Користувач 2 | × (очікування 0.4с)
Повідомлення 12 | Користувач 3 | × (очікування 0.4с)
Повідомлення 13 | Користувач 4 | × (очікування 0.9с)
Повідомлення 14 | Користувач 5 | × (очікування 0.7с)
Повідомлення 15 | Користувач 1 | × (очікування 0.7с)
Повідомлення 16 | Користувач 2 | ✓
Повідомлення 17 | Користувач 3 | ✓
Повідомлення 18 | Користувач 4 | ✓
Повідомлення 19 | Користувач 5 | ✓
Повідомлення 20 | Користувач 1 | ✓
```

## ThrottlingRateLimiter

File [throttling_rate_limiter.py](./throttling_rate_limiter.py) contains the implementation of the throttling rate limiter class.
Can be checked by build-in test cases in the file

```sh
python throttling_rate_limiter.py
```

Output:

```log
=== Симуляція потоку повідомлень (Throttling) ===
Повідомлення  1 | Користувач 2 | ✓
Повідомлення  2 | Користувач 3 | ✓
Повідомлення  3 | Користувач 4 | ✓
Повідомлення  4 | Користувач 5 | ✓
Повідомлення  5 | Користувач 1 | ✓
Повідомлення  6 | Користувач 2 | × (очікування 5.9с)
Повідомлення  7 | Користувач 3 | × (очікування 5.6с)
Повідомлення  8 | Користувач 4 | × (очікування 5.7с)
Повідомлення  9 | Користувач 5 | × (очікування 6.0с)
Повідомлення 10 | Користувач 1 | × (очікування 6.7с)

Очікуємо 10 секунд...

=== Нова серія повідомлень після очікування ===
Повідомлення 11 | Користувач 2 | ✓
Повідомлення 12 | Користувач 3 | ✓
Повідомлення 13 | Користувач 4 | ✓
Повідомлення 14 | Користувач 5 | ✓
Повідомлення 15 | Користувач 1 | ✓
Повідомлення 16 | Користувач 2 | × (очікування 6.4с)
Повідомлення 17 | Користувач 3 | × (очікування 6.5с)
Повідомлення 18 | Користувач 4 | × (очікування 6.3с)
Повідомлення 19 | Користувач 5 | × (очікування 6.7с)
Повідомлення 20 | Користувач 1 | × (очікування 6.4с)
```
