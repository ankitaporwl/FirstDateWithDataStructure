#include<bits/stdc++.h>
using namespace std;
#define size 5
int Linear_Queue[size];
int front=0;
int rear=0;
bool isfull(){
	if(rear==size){
		return true;
	}else{
		return false;
	}
}
bool isempty(){
	if(front==size){
		return true;
	}else{
		return false;
	}
}
void EnQueue(int data){
	if(isfull()){
		cout<<"overflow";
	}else{
		Linear_Queue[rear]=data;
		rear++;
	}
}
void DeQueue(){
	if(isempty()){
		cout<<"underflow";
	}else{
		
		int del_element=Linear_Queue[front];
		cout<<"deleted element:"<<endl;
		cout<<del_element<<endl;
		front++;
		if(front==rear){
			front=0;
			rear=0;
		}
	}
}
void front_element(){
	if(isempty()){
		cout<<"underflow"<<endl;
	}else{
		cout<<"front element is:"<<Linear_Queue[front]<<endl;
	}
}
void rear_element(){
	if(isempty()){
		cout<<"underflow"<<endl;
	}else{
		cout<<"rear element:"<<Linear_Queue[rear-1]<<endl;
	}
}
void display(){
	if(isempty()){
		cout<<"underflow"<<endl;
	}else{
		cout<<"elements in linear queue:"<<endl;
		for(int i=front;i<rear;i++){
			cout<<Linear_Queue[i]<<" ";
		}
		cout<<endl;
	}
}
int main(){
	EnQueue(1);
	EnQueue(2);
	EnQueue(3);
	EnQueue(4);
	EnQueue(5);
	
	DeQueue();
	DeQueue();
	
	display();
	front_element();
	rear_element();
	
	cout<<"queue is full"<<endl;
	EnQueue(6);
	return 0;
}
