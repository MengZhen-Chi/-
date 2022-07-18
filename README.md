# -
字节跳动作业

#第一次作业
1
App的生命周期：
Notrunning→Inactive↔Active\Background↔Suspended→Notrunning
              


ViewController的生命周期：alloc/init、loadView、viewDidLoad、viewWillAppear、viewDidAppear、viewWillDisappear、viewDidDisppear、dealloc

2
五种常用的UI控件：
Uiscrollview、UITableview、UIColectionview、UIWebview、UIViewController

3
(1).定义每个UITableView中的cell的行高

- (CGFloat)tableView:(UITableView *)tableView heightForRowAtIndexPath:(NSIndexPath *)indexPath
{
    // indexPath.section,根据分组进行更精确的配置
    return 90.0;
}

(2).设置UITableView每个分组的Header的Title

- (NSString *)tableView:(UITableView *)tableView titleForHeaderInSection:(NSInteger)section{
    return [_arrayType objectAtIndex:section];
    
}

(3).设置UITableView分组Header的高

- (CGFloat)tableView:(UITableView *)tableView heightForHeaderInSection:(NSInteger)section{
    return 30.0;
}


#第二次作业

#类的声明

@interface Student:NSObject{

    @public
    
    NSString* name;
    
    NSString* major;
    
    int age;
}

#方法

-(void) study:(float) time;

@end

#类的实现

@implementation Student

-(void) study:(float) time{

NSLog(@"The study time of the student is %@", time);

@end




