# twitter_parser
There is free python-based parser of <https://twitter.com> that allows to parse any date-range by any word or phrase. 

Also, Parser has parameters to filter by language, location and etc. Good Luck with using!   

Usage:


    if __name__ == "__main__":
        # WARNING: SEARCH WITH WORDS FIND ALSO USERS AND REPLIES WITH THIS WORDS
        #query: list with operators for search:
        #    str, all words in tweet: 'word1 word2 word3'
        #    str, words in exact phrase: '"word1 word2 word3"'
        #    str, any of the words: 'word1 OR word2 OR word3'
        #    str, none of the words: '-word1 -word2 -word3'
        #    str, hashtags: '#word1 OR #word2 OR #word3'
        #    str, from people: 'from:word1 OR from:word2 OR from:word3'
        #    str, to people: 'to:word1 OR to:word2 OR to:word3'
        #    str, with people: '@word1 OR @word2 OR @word3'
        query = ["Ford"]
        print(query)
        parse_twitter(query=query, since='2010-03-19', days=3, _name='Ford')

