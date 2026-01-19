// Jackie
// Lab 1
// 1/18/2026
#define _POSIX_C_SOURCE 200809L
#include <stdio.h>
#include <stdlib.h>
#include <string.h>

int main() {
  char *user_input = NULL;
  size_t size = 0;

  printf("Please enter some text: "); // get user input (string)
  ssize_t line = getline(&user_input, &size, stdin);

  if (line == -1) { // checking if getline worked
    perror("getline failed");
    exit(EXIT_FAILURE);
  }

  char *wordptr;
  char *current_token = strkok_r(user_input, " ", &wordptr);

  while (current_token != NULL) {
    printf("Tokens: \n %s \n", current_token);
    current_token = strkok_r(NULL, " ", &wordptr);
  }
  free(user_input);

  return 0;
}
