#sigverse header
SIG_SRC  = $(SIGVERSE_PATH)/include/sigverse

#オブジェクトファイルの指定
#OBJS     = Test.so TrashBox.so Camera.so Wagon.so Moderator.so
OBJS     = EGPSR2015Robo.so Moderator.so Human_agent.so
#OBJS     = CleanUpRoboDemo.so TrashBox.so Camera.so Wagon.so Moderator.so
#OBJS     = Test.so TrashBox.so Furniture.so Camera.so Wagon.so Moderator.so

all: $(OBJS)

#compile
./%.so: ./%.cpp
	g++ -DCONTROLLER -DNDEBUG -DUSE_ODE -DdDOUBLE -I$(SIG_SRC) -I$(SIG_SRC)/comm/controller -fPIC -shared -o $@ $<

clean:
	rm ./*.so
