## Assignments

### Week 1

1. [k-Nearest Neighbor classifier](https://github.com/xenohunter/cs231n/commit/80ccfc674d44e1237e8d4e05aa8b5569cf71abec)
2. [Training a Support Vector Machine](https://github.com/xenohunter/cs231n/commit/d4197d7d4544ca17c070ab9597e61f8870f7c995)
3. [Implement a Softmax classifier](https://github.com/xenohunter/cs231n/commit/83edcd0fa80e7ee9c29676603389772359c7be19)
4. [Two-Layer Neural Network](https://github.com/xenohunter/cs231n/commit/abc500d80d74948f36ec720ef205b62077e79e7a)
5. [Higher Level Representations: Image Features](https://github.com/xenohunter/cs231n/commit/8acd81cc301b601d9fa0fca7ad805a8245691904)

### Week 2

1. [Fully-connected Neural Network](https://github.com/xenohunter/cs231n/commit/70542f6fb3f112aec0b0d63dfa96ca2582002eca)
2. [Batch Normalization](https://github.com/xenohunter/cs231n/commit/255ffe3c39509baf7d352a1039c52ce5a3c2a2b8)

## Troubleshooting

### Missing libstdc++.so.6

In case you're getting this error when running `jupyter notebook`:

```
ImportError: /home/xenohunter/.local/share/anaconda3/envs/cs231n/lib/libstdc++.so.6:
version `GLIBCXX_3.4.29' not found (required by /usr/lib/libzmq.so.5)
```

Go to the Anaconda environment directory and link the file from `/usr/lib`:

```
cd .local/share/anaconda3/envs/cs231n/lib/
mv -vf libstdc++.so.6 libstdc++.so.6.old
ln -s /usr/lib/libstdc++.so.6 ./libstdc++.so.6
```

Credits due to [this answer](https://askubuntu.com/questions/575505/glibcxx-3-4-20-not-found-how-to-fix-this-error/764572#764572).
