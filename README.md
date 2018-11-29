# rn-refresh-anim
install
--------
npm i refresh-anim-dugz

------
base usage
----
```javascript
 <View style={{
        alignItems: "center",
        justifyContent: "center",
        backgroundColor: "pink"
      }}>
        <Text>
          when RefreshAnimView received props initState='start',
          it will begin to rotate during to show.
        </Text>
        <RefreshAnimView ref='refreshAnimView' initState='start'/>

        <TouchableOpacity
          activeOpacity={0.7}
          onPress={() => {
            this.refs.refreshAnimView && this.refs.refreshAnimView.startAnim();
          }}>
          <Text>
            start
          </Text>
        </TouchableOpacity>

        <TouchableOpacity
          activeOpacity={0.7}
          onPress={() => {
            this.refs.refreshAnimView && this.refs.refreshAnimView.restartAnim();
          }}>
          <Text>
            restart
          </Text>
        </TouchableOpacity>

        <TouchableOpacity
          activeOpacity={0.7}
          onPress={() => {
            this.refs.refreshAnimView && this.refs.refreshAnimView.stopAnim();
          }}>
          <Text>
            stop
          </Text>
        </TouchableOpacity>
      </View>
```
--------

