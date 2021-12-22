build:  ## target create site hugo
	@hugo > /dev/null
.PHONY: clean 
clean:  ## remove all from dist
	@rm -r dist/* > /dev/null 
post:	## create post

    ifdef $(and POST_NAME, POST_TITLE)
 	    @hugo new posts/"${POST_NAME}.md" > /dev/null
	    @sed -i "s/${POST_NAME}/${POST_TITLE}/gi" "./content/posts/${POST_NAME}.md"
    endif