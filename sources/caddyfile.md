# Peach's blog

www.peachis.me, peachis.me {
proxy / http://127.0.0.1:2368 {
transparent
}
redir 301 {
/fix-the-games-which-use-wineskin-on-ei-caption /fix-the-games-which-use-wineskin-on-ei-capitan/
/fix-the-games-which-use-wineskin-on-ei-caption/ /fix-the-games-which-use-wineskin-on-ei-capitan/
}
gzip
}

# Tommao's book site

http://books.codingcat.top {
root /data/tommao/www/books/site
gzip
}

# Tommao's codingcat

http://www.codingcat.top, http://codingcat.top {
proxy / http://127.0.0.1:8005 {
transparent
except /dist
}
root /data/tommao/www/codingcat/web
gzip

}

# Tommao's feeder

http://feeder.codingcat.top {
proxy / http://127.0.0.1:8018 {
transparent
except /static
}
root /data/tommao/feeder/feeder
gzip

}
