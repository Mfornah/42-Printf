# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: mfornah <mfornah@student.42.fr>            +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2022/10/21 17:09:02 by mfornah           #+#    #+#              #
#    Updated: 2022/12/01 15:45:44 by mfornah          ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

NAME = libftprintf.a
CC    = gcc
CFLAGS   = -Werror -Wall -Wextra
AR = @ar rcs

SRC = ft_checkparam.c ft_hexpointer.c ft_print_pa.c \
		ft_print_putchar.c ft_print_putstr.c ft_print_unsingened.c\
		ft_printf_hexlong.c ft_printf_ptr.c ft_printf_putnbr.c \
		ft_printf.c ft_putnbr_base_uns.c ft_strlen2.c ft_checkbase.c\


OBJS = $(SRC:.c=.o)

$(NAME) : $(OBJS) 
	$(AR) $(NAME) $(OBJS)

RM = rm -f

all: $(NAME)

%.o : %.c
	$(CC) $(CFLAGS) -c -o $@ $<

clean:
	$(RM) $(OBJS) 

fclean: clean
	$(RM) $(NAME) $(OBJS)

re: fclean all

.PHONY: all re clean fclean 