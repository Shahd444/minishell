CC = cc
NAME = libft.a
CFLAGS = -Wall -Wextra -Werror -g

SRC = ft_atoi.c\
      ft_bzero.c\
      ft_isalnum.c\
      ft_isalpha.c\
      ft_isascii.c\
      ft_isdigit.c\
      ft_isprint.c\
      ft_memchr.c\
      ft_memcmp.c\
      ft_memcpy.c\
      ft_memmove.c\
      ft_memset.c\
      ft_strchr.c\
      ft_strlen.c\
      ft_strncmp.c\
      ft_strnstr.c\
      ft_strrchr.c\
      ft_tolower.c\
      ft_toupper.c\
      ft_strlcpy.c\
      ft_strlcat.c\
      ft_calloc.c\
      ft_strdup.c\
      ft_substr.c\
      ft_putchar_fd.c\
      ft_putendl_fd.c\
      ft_putstr_fd.c\
      ft_strjoin.c\
      ft_strtrim.c\
      ft_itoa.c\
      ft_strmapi.c\
      ft_striteri.c\
      ft_putnbr_fd.c\
      ft_split.c\
      ft_print_char.c\
      ft_print_str.c\
      ft_print_udigit.c\
      ft_print_sdigit.c\
      ft_print_address.c\
      ft_printf.c\
      get_next_line.c\
      ft_strcmp.c\
      ft_atol.c\
      ft_strcpy.c\
      ft_strcat.c\
      ft_strndup.c\
      ft_is_spaces.c\

SRC_BONUS = ft_lstnew.c\
	ft_lstadd_front.c\
	ft_lstsize.c\
	ft_lstlast.c\
	ft_lstadd_back.c\
	ft_lstdelone.c\
	ft_lstclear.c\
	ft_lstiter.c\
      ft_lstmap.c\


OBJ = $(SRC:.c=.o)
OBJ_BONUS = $(SRC_BONUS:.c=.o)

all: $(NAME)

$(NAME): $(OBJ)
	ar rcs $(NAME) $(OBJ)

%.o: %.c
	$(CC) $(CFLAGS) -c $< -o $@
	
bonus: $(OBJ) $(OBJ_BONUS)
	ar rcs $(NAME) $(OBJ) $(OBJ_BONUS)

clean:
	rm -f $(OBJ) $(OBJ_BONUS)

fclean: clean
	rm -f $(NAME)

re: fclean all

.PHONY: all clean fclean bonus re
