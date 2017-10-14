# Intellect-User-Creation
Creating a java standalone application to add , update and delete the user


package com.pack.intellect;

import java.util.ArrayList;

public class CreateUser {

	public ArrayList methodCreate(){
		
		UserDetailsBean bean = null;
		ArrayList ls = new ArrayList();
		bean = new UserDetailsBean();
	    bean.setId("1528236");
	    bean.setfName("Deva");
	    bean.setlName("Guru");
	    bean.setEmail("deva.guru@gmail.com");
	    bean.setPincode(600047);
	    bean.setBirthDate("09/01/1992");
	    bean.setActive(true);
	    ls.add(bean);
	    
	    bean = new UserDetailsBean();
	    bean.setId("1528237");
	    bean.setfName("Desy");
	    bean.setlName("Angel");
	    bean.setEmail("desy.angel@gmail.com");
	    bean.setPincode(600046);
	    bean.setBirthDate("08/01/1992");
	    bean.setActive(true);
	    ls.add(bean);
	    
	    bean = new UserDetailsBean();
	    bean.setId("1528238");
	    bean.setfName("bob");
	    bean.setlName("brady");
	    bean.setEmail("bob.brady@gmail.com");
	    bean.setPincode(600045);
	    bean.setBirthDate("08/01/1992");
	    bean.setActive(true);
	    ls.add(bean);
	    
	    
	    
	    return ls;

	    
	}
	
	public static void main(String arg[]){
		
		ArrayList ls = new ArrayList();
		CreateUser user = new CreateUser();
		UpdateUser userUpdate = new UpdateUser();
		DeleteUser deleteUser = new DeleteUser();
		ls = user.methodCreate();
		userUpdate.updateMethod(ls);
		deleteUser.invalidateUser(ls);
		
	}
	
	
	
}

