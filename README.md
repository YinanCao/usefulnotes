# usefulnotes
- git add *; git commit -m 'xxx'; git push;
- cd ~ to enter home directory;
  - open -e .bash_profile
    - alias ukelog='ssh -YCX yinancao@172.18.101.96'
      - killall Finder
- display IP address: ip addr (ip a)
- ls -alhtrp --group-directories-first --color=always
- echo "bind '"\e[A": history-search-backward'" >> .bashrc
  - echo "bind '"\e[B": history-search-forward'" >> .bashrc
    - source .bashrc
- ssh -X to higher nodes
- rsync -davP --ignore-existing --exclude '*.edf'

# Binomial Likelihood Function
say you L(p|n,h) = nchoosek(n,h)*(p.^h)*((1-p).^(n-h)); often, we fit model to single trial data, so h = 0/1, and n = 1, so the coefficient = 1;
the log-likelihood: LL = log(p.^h) + log((1-p).^(n-h))
