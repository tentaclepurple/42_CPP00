# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: codespace <codespace@student.42.fr>        +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2023/11/03 17:10:07 by imontero          #+#    #+#              #
#    Updated: 2023/11/12 00:35:28 by codespace        ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

NAME = acc

FLAGS = -Wall -Wextra -Werror -std=c++98 -pedantic

CC = g++

INCLUDE = 	Account.hpp

SRC_FILES = Account.cpp \
			tests.cpp	
		
OBJS = $(SRC_FILES:.cpp=.o)

CLR_RMV		:= \033[0m
RED		    := \033[1;31m
GREEN		:= \033[1;32m
YELLOW		:= \033[1;33m
BLUE		:= \033[1;34m
CYAN 		:= \033[1;36m

define	ART
$(RED)                                                        
                                                 
                                           
                     █                     
                    ███                    
                    ███                    
                   █████                   
                  ██████                   
                  ███████                  
                 █████████                 
   █████████████████████████████████████   
     █████████████████████████████████     
       █████████████████████████████       
          ███████████████████████          
            ███████████████████            
              ███████████████              
             █████████████████             
            ███████████████████            
            ████████  █████████            
           ███████       ███████           
           ████             ████           
          ███                 ███    
		        

      ___           ___           ___     
     /\  \         /\  \         /\  \    
    /::\  \       /::\  \       /::\  \   
   /:/\:\  \     /:/\:\  \     /:/\:\  \  
  /:/  \:\  \   /::\~\:\  \   /::\~\:\  \ 
 /:/__/ \:\__\ /:/\:\ \:\__\ /:/\:\ \:\__\ 
 \:\  \  \/__/ \/__\:\/:/  / \/__\:\/:/  / 
  \:\  \            \::/  /       \::/  /  
   \:\  \            \/__/         \/__/   
    \:\__\                                
     \/__/                                

 $(CLR_RMV)
endef
export	ART

all: $(NAME)

$(NAME): $(OBJS) $(INCLUDE)
	@$(CC) $(FLAGS) $(OBJS) -o $(NAME)
	@echo "$$ART"

clean:
	@rm -f $(OBJS)

fclean: clean
	@rm -f $(NAME)

re: fclean all

.PHONY: all clean fclean re