# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: aanouari <aanouari@student.42.fr>          +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2022/10/26 21:54:11 by aanouari          #+#    #+#              #
#    Updated: 2022/11/11 13:05:57 by aanouari         ###   ########.fr        #
#                                                                              #
# **************************************************************************** #


NAME = libft.a


SRCS =		ft_isalpha.c		ft_isdigit.c		ft_isascii.c		ft_isalnum.c		ft_isprint.c		ft_strlen.c			\
			ft_memset.c			ft_bzero.c			ft_memcpy.c			ft_memmove.c		ft_strlcpy.c		ft_strlcat.c		\
			ft_toupper.c		ft_tolower.c		ft_strchr.c			ft_strrchr.c		ft_strncmp.c		ft_memchr.c			\
			ft_memcmp.c			ft_strnstr.c		ft_atoi.c			ft_calloc.c			ft_strdup.c			ft_substr.c			\
			ft_strjoin.c		ft_strtrim.c		ft_split.c			ft_itoa.c			ft_strmapi.c		ft_striteri.c		\
			ft_putchar_fd.c		ft_putstr_fd.c		ft_putendl_fd.c		ft_putnbr_fd.c


OBJ_S = $(SRCS:.c=.o)


BONUS = 	ft_lstnew_bonus.c	 	ft_lstadd_front_bonus.c		ft_lstsize_bonus.c		ft_lstlast_bonus.c		ft_lstadd_back_bonus.c \
			ft_lstdelone_bonus.c	ft_lstclear_bonus.c			ft_lstiter_bonus.c		ft_lstmap_bonus.c


OBJ_B = $(BONUS:.c=.o)


CC = cc


CFLAGS =  -Wall -Wextra -Werror


RM = rm -rf


all:			$(NAME)


$(NAME):		$(OBJ_S)
				ar rc $(NAME) $(OBJ_S)


bonus:			$(OBJ_B) $(OBJ_S)
				ar rc $(NAME) $(OBJ_B) $(OBJ_S)


clean:
				$(RM) $(OBJ_S) $(OBJ_B)


fclean:			clean
				$(RM) $(NAME)


re:				fclean all
