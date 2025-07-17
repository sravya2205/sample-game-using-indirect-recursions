def Player_A(n):
    if n<=0:
        print("player A reached 0!! player a losses")
        return
    print(f"\n player A's turn.Current number {n}")
    move=int(input("player a ,subtract 1 or 2:"))
    while move not in [1,2]:
        move=int(input("Player a,subtact 1 or 2:"))
    player_B(n-move)
def player_B(n):
    if n<=0:
        print("player b reached 0!! player b loss")
        return
    print(f"\n player b's turn.Current number{n}")
    move=int(input("player a ,subtract 1 or 2:"))
    while move not in [1,2]:
        move=int(input("Player b,subtact 1 or 2:"))
    Player_A(n-move)
start=int(input("enter a number:"))
Player_A(start)
