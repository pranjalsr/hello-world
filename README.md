# hello-world
Just another Repository
import java.util.List;

public class Movies {
	
	private int movie_id;
	private String release_date;
	private long box_office_budget;
	private String[] songs= new String[5];
	public Movies(){
		
	}
	
	public Movies(int movie_id, String release_date, long box_office_budget, String[] songs) {
	//	super();
		this.movie_id = movie_id;
		this.release_date = release_date;
		this.box_office_budget = box_office_budget;
		this.songs = songs;
	}

	public int getMovie_id() {
		return movie_id;
	}

	public void setMovie_id(int movie_id) {
		this.movie_id = movie_id;
	}

	public String getRelease_date() {
		return release_date;
	}

	public void setRelease_date(String release_date) {
		this.release_date = release_date;
	}

	public long getBox_office_budget() {
		return box_office_budget;
	}

	public void setBox_office_budget(long box_office_budget) {
		this.box_office_budget = box_office_budget;
	}

	public String[] getSongs() {
		return songs;
	}

	public void setSongs(String[] songs) {
		this.songs = songs;
	}
	
	public static  void display(Movies m){
		System.out.println("Movie Id is" +m.getMovie_id());
		System.out.println(m.getRelease_date());
		System.out.println(m.getBox_office_budget());
		for(int i=0;i<m.getSongs().length;i++)
		{
			System.out.println(m.getSongs()[i]);
		}
	}
	public static void main(String [] arg){
		String[] movies_song= {"1","34","sdjhfksjd","sdjkfh","sdjfhk"};
			Movies m1=new Movies();
			m1.setMovie_id(1);
			m1.setRelease_date("12/05/2018");
			m1.setBox_office_budget(5000000l);
			m1.setSongs(movies_song);
			display(m1);
	}
	
	
	
}
