# Burrow Bypass
burrow bypass for crystalpvp.cc

## Tutorial
Heres a tutorial on how to bypass crystalpvp.cc plugins and burrow

1. Find any public burrow source code
2. Replace its rubberband method with 
```java
for (int i = 0; i < 20; i++)
  mc.player.networkHandler.sendPacket(new PlayerMoveC2SPacket.PositionAndOnGround(mc.player.getX(), mc.player.getY() + 1337, mc.player.getZ(), false));
```
or with this on 1.12 forge
```java
for (int i = 0; i < 20; i++)
  mc.player.connection.sendPacket(new CPacketPlayer.Position(mc.player.posX, mc.player.posY + 1337, mc.player.posZ, false));
```
3. Ur golden

## Credits
lemoliam (hes cool)
