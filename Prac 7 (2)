#include <stdio.h>
#include <string.h>

int indexOf(char text[], char word[]) {
    int textLen = strlen(text);
    int wordLen = strlen(word);
    
    if (wordLen == 0 || wordLen > textLen) {
        return -1;
    }

    for (int i = 0; i <= textLen - wordLen; i++) {
        int j;
        for (j = 0; j < wordLen; j++) {
            if (text[i + j] != word[j]) {
                break;
            }
        }
        if (j == wordLen) {
            return i;
        }
    }
    return -1;
}

int main() {
    char sentence[] = "The cat sat on the mat";
    char word[] = "cat";
    
    int position = indexOf(sentence, word);
    
    if (position != -1) {
        printf("Слово \"%s\" найдено на позиции: %d\n", word, position);
    } else {
        printf("Слово \"%s\" не найдено.\n", word);
    }
    
    return 0;
}
