# Flutter Course Code

## Getting Started

#task1,
import 'package:flutter/material.dart';
class buildInstagram extends statefullWidget(){
   @override
  _buildHreart createState() => _buildHreart2();
}

class _buildHreart extends State<buildInstagram> {
  @override
  Widget build(BuildContext context) {
    return Sacfold(
      backgroundColor:Colors.white,
      body:listView( physics:AlwaysScrolableScrolPhysics(),
        children:<Widget>[
          Row(
            mainAxiesAlignment:MainAxiesAlignment.spaceBetween,
            children:[Text(
              'Instagram',
              style: TextStyle(
                fontSize: 24,
                fontFamily: 'brillaborg',
                color: Colors.black,
              ),
            ),],
            Row(
            children:[
              iconButton(icon:Icons.live_tv,
              iconSize=30.0,
              onPressed:(){},),
             SizedBox(width 16.0),
             container(
              iconButton(icon:Icons.send,
              iconSize=30.0,
              onPressed:(){print("Direct Message"),},),),),
            ],
          ),
        ],
        container(
          width:double.infinity,
          height:100.0,
          color:Colors.white,
          child:listView.builder(
            scrollDirection:Axis.horizontal;
            itemCount:Stories.length+1,
            itemBuilder:(BuildContext context,int index),
            if(index==1){
              return SizedBox(weidth:10.0),
            }
            Padding(
           return Container(
                  margin: EdgeInsets.all(10.0),
                  width: 60.0,
                  height: 60.0,
                  decoration: BoxDecoration(
                    shape: BoxShape.circle,
                    boxShadow: [
                      BoxShadow(
                        color: Colors.black45,
                        offset: Offset(0, 2),
                        blurRadius: 6.0,
                      ),
                    ],
                  ),
                  child: CircleAvatar(
                    child: ClipOval(
                      child: Image(
                        height: 60.0,
                        width: 60.0,
                        image: AssetImage(stories[index - 1]),
                        fit: BoxFit.cover,
                      ),
                    ),
                  ),
                   Padding( padding:EdgeInsets.symmetric(,horizontal:10.0,vertical: 10.0),
                   child:Container(
                  
                       width: double.infinity,
                     height: 560.0,
                     decoration:BoxDecoration(
                     color:Colors.white,
                     borderRadius:BorderRadius.Circle(20.0),
                      ),
                         padding: EdgeInsets.symmetric(vertical: 10.0),
                     child:column(
                       children:<Widget>[
                         child:ListTile(
                          leading:Container(
                  margin: EdgeInsets.all(10.0),
                  width: 60.0,
                  height: 60.0,
                  decoration: BoxDecoration(
                    shape: BoxShape.circle,
                    boxShadow: [
                      BoxShadow(
                        color: Colors.black45,
                        offset: Offset(0, 2),
                        blurRadius: 6.0,
                      ),
                    ],
                  ),
                  child: CircleAvatar(
                    child: ClipOval(
                      child: Image(
                        height: 60.0,
                        width: 60.0,
                        image: AssetImage(stories[index - 1]),
                        fit: BoxFit.cover,
                      ),
                    ),
                  ),
                  Title:text(post[0].authername,style: TextStyle(
                        fontSize: 24,
                        fontWeight: FontWeight.bold,
                          color: Colors.black,),
                         ),
                  subtitle:Text(post[0].timeAgo),
                  trailing:IconButton(
                    icon:Icon(Icons.more.horizantle),
                    color: Colors.black,),
                    onPressed:(){print('more'),}
                  ),
                       ],
                     ),
                      Container(
                  margin: EdgeInsets.all(10.0),
                  width: double.infinity,
                  height: 400.0,
                  decoration: BoxDecoration(
                    shape: BoxShape.circle,
                    boxShadow: [
                      BoxShadow(
                        color: Colors.black45,
                        offset: Offset(0, 5),
                        blurRadius: 8.0,
                      ),
                    ],
                    image:DecorationImage(image:assetImage[post[0].imageURL],),
                    fit:Boxfit.fitWidth,
                  ), ),
                                          Padding(
                          padding: EdgeInsets.symmetric(horizontal: 20.0),
                          child: Row(
                            mainAxisAlignment: MainAxisAlignment.spaceBetween,
                            children: <Widget>[
                              Row(
                                children: <Widget>[
                                  Row(
                                    children: <Widget>[
                                      IconButton(
                                        icon: Icon(Icons.favorite_border),
                                        iconSize: 30.0,
                                        onPressed: () => print('Like post'),
                                      ),
                                      Text(
                                        '2,515',
                                        style: TextStyle(
                                          fontSize: 14.0,
                                          fontWeight: FontWeight.w600,
                                        ),
                                      ),
                                    ],
                                  ),
                                  SizedBox(width: 20.0),
                                  Row(
                                    children: <Widget>[
                                      IconButton(
                                        icon: Icon(Icons.chat),
                                        iconSize: 30.0,
                                        onPressed: () {
                                          print('Chat');
                                        },
                                      ),
                                      Text(
                                        '350',
                                        style: TextStyle(
                                          fontSize: 14.0,
                                          fontWeight: FontWeight.w600,
                                        ),
                                      ),
                                    ],
                                  ),
                                ],
                              ),
                              IconButton(
                                icon: Icon(Icons.bookmark_border),
                                iconSize: 30.0,
                                onPressed: () => print('Save post'),
                              ),
                            ],
                          ),
                        ),
                      ],
                    ),
                  ),
                ],
              ),
            ),
                ),
              },
            ),
          )
             _buildPost(0),
          _buildPost(1),
          ),

      ),
     bottomNavigationBar: ClipRRect(
        borderRadius: BorderRadius.only(
          topLeft: Radius.circular(30.0),
          topRight: Radius.circular(30.0),
        ),
        child: BottomNavigationBar(
          type: BottomNavigationBarType.fixed,
          items: [
            BottomNavigationBarItem(
              icon: Icon(
                Icons.dashboard,
                size: 30.0,
                color: Colors.black,
              ),
              title: Text(''),
            ),
            BottomNavigationBarItem(
              icon: Icon(
                Icons.search,
                size: 30.0,
                color: Colors.grey,
              ),
              title: Text(''),
            ),
            
            BottomNavigationBarItem(
              icon: Icon(
                Icons.favorite_border,
                size: 30.0,
                color: Colors.grey,
              ),
              title: Text(''),
            ),
            BottomNavigationBarItem(
              icon: Icon(
                Icons.person_outline,
                size: 30.0,
                color: Colors.grey,
              ),
              title: Text(''),
            ),
          ],
        ),
      ),
    );
  }
}

//___-main-----------------------
  
import 'package:flutter/material.dart';
import 'package:flutter/buildInstagram.dart';

void main() => runApp(MyApp());

class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      title: 'Flutter Demo',
      debugShowCheckedModeBanner: false,
      theme: ThemeData(
        primarySwatch: Colors.blue,
      ),
      home: const buildInstagram(title: 'Flutter Demo Home Page'),
    );
  }
}

class Post {
  String authorName;
  String authorImageUrl;
  String timeAgo;
  String imageUrl;

  Post({
    this.authorName,
    this.authorImageUrl,
    this.timeAgo,
    this.imageUrl,
  });
}

final List<Post> posts = [
  Post(
    authorName: 'fatima ',
    authorImageUrl: 'assets/images/photo_1.jpg',
    timeAgo: '5 min',
    imageUrl: 'assets/images/photo_1.jpg',
  ),
  Post(
    authorName: 'noor Martin',
    authorImageUrl: 'assets/images/image.png',
    timeAgo: '10 min',
    imageUrl: 'assets/images/photo_4.jpg',
  ),
  Post(
    authorName: 'noor Martin',
    authorImageUrl: 'assets/images/photo_1.png',
    timeAgo: '10 min',
    imageUrl: 'assets/images/photo_5.jpg',
  ),
];

final List<String> stories = [
  'assets/images/image.png',
  'assets/images/photo_3.jpg',
  'assets/images/photo_4.jpg',
  'assets/images/photo_5.jpg',
];
