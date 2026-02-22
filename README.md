#include <stdio.h>
#include <stdlib.h>

struct node {
    int data;
    struct node* next;
};

int main() {
    struct node *head = NULL, *newNode;

    newNode = (struct node*)malloc(sizeof(struct node));
    printf("Enter data to insert at beginning: ");
    scanf("%d", &newNode->data);

    newNode->next = head;
    head = newNode;

    printf("New head data: %d", head->data);

    return 0;
}
